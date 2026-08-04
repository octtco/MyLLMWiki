---
type: output
output_type: qa
status: reusable
promote_to_wiki: false
question: Hermes、Claude Code 和 Codex 能否通过 TencentDB-Agent-Memory 共享本地项目记忆
scope: 评估三个本地 Agent 共享记忆、工作摘要和主控 Agent 查询能力的最小架构
source_pages: []
related_topics:
  - Agent 框架设计
  - Agent 记忆与知识图谱
  - AI 工具化知识工作流
related_concepts: []
updated: 2026-08-03
---

# Hermes、Claude Code 和 Codex 能否共享本地项目记忆

## 短答案

可以，但不是安装后三个 Agent 就会自动共享全部上下文。

最小可行方案是让 Hermes、Claude Code 和 Codex 都连接同一个本地 MemoryCore Gateway，并用统一的 `team_id`、`user_id` 和项目标识共享项目记忆，同时为每个 Agent 保留独立的 `agent_id`。每个 Agent 在任务结束时写入结构化工作摘要，主控 Agent 再查询这些摘要。

## 展开

推荐的基础结构是：

```text
Hermes ─────┐
Claude Code ─┼─> 本地 MemoryCore Gateway ─> 共享记忆 / 项目知识
Codex ──────┘                         ↑
                                 主控 Agent 查询
```

三个 Agent 可以共享项目背景、技术约束、架构决策、历史任务、Skill、Wiki 和 CodeGraph。更适合共享的是经过整理的项目事实和工作结果，而不是三套完整聊天记录。

Hermes 可以使用仓库提供的适配器；Claude Code 和 Codex 需要通过 TypeScript / Python SDK、HTTP API 或 MCP 增加轻量接入层。接入层至少需要完成两件事：

1. 在任务结束时写入对话或结构化工作摘要。
2. 在生成下一轮 Prompt 前，读取相关的项目记忆、场景和任务状态。

建议的任务摘要包含：

```json
{
  "project": "my-project",
  "agent_id": "claude-code",
  "task_id": "auth-refactor-001",
  "status": "completed",
  "changed_files": ["src/auth.ts", "src/session.ts"],
  "decisions": ["保留旧登录接口，移动端仍在使用"],
  "tests": ["npm test"],
  "blockers": [],
  "next_steps": ["Codex 检查移动端兼容性"]
}
```

身份隔离可以采用：

```text
team_id = my-project
user_id = lelele
agent_id = hermes
agent_id = claude-code
agent_id = codex
```

这样既能共享团队级项目记忆，也不会把三个 Agent 的个人记忆混成一处。具体共享范围还应结合 `private`、`team`、`restricted` 和 Agent 绑定关系控制。

## 主控 Agent 能知道什么

只要其他 Agent 有上报，主控 Agent 可以查询：

- 谁执行了什么任务；
- 修改了哪些文件；
- 做过哪些架构决策；
- 测试是否通过；
- 当前有哪些阻塞；
- 下一步应该由哪个 Agent 接手。

但 MemoryCore 本身不是调度器。它不会自动决定任务分派、检测代码冲突，也不会判断两个 Agent 的结论谁更可靠。主控逻辑、任务锁和代码协作规则仍需单独实现。

## 推荐的最小闭环

```text
1. 本地启动 MemoryCore Gateway
2. Hermes 使用现有适配器接入
3. Claude Code 和 Codex 通过 SDK / HTTP / MCP 接入
4. 每个任务结束写入工作摘要
5. 主控 Agent 查询项目记忆和其他 Agent 的任务摘要
6. 验证共享记忆确实改善了下一次任务的冷启动
```

第一阶段不建议同步所有原始上下文。先共享“项目事实、决策、改动文件、测试结果和阻塞项”，更容易控制噪声、权限和错误记忆传播。

## 依据

- [TencentDB-Agent-Memory README](https://github.com/TencentCloud/TencentDB-Agent-Memory)：说明 MemoryCore、Chat Memory、Skill、Wiki、CodeGraph 和多 Agent 资产绑定。
- [MemoryCore OpenClaw 架构说明](https://github.com/TencentCloud/TencentDB-Agent-Memory/blob/feat/server_team/MemoryCore/openclaw-plugin/docs/architecture.md)：说明 OpenClaw 客户端适配器、Gateway、SDK 和远端存储的分层。
- [Python SDK v3](https://github.com/TencentCloud/TencentDB-Agent-Memory/blob/feat/server_team/sdk/memory-core/python/tencentdb_agent_memory/v3/client.py)：说明 `team_id`、`agent_id`、`user_id`、`session_id` 等隔离维度，以及 L0-L3 的 API。

## 当前边界

- 当前仓库对 OpenClaw 和 Hermes 有现成接入路径；Claude Code 和 Codex 的适配仍需要自行补齐。
- 共享记忆是最终一致的，L1、L2、L3 的抽取和归纳可能存在延迟。
- Agent 断开 MemoryCore 时，当前客户端模式不会自动提供完整的本地离线回退。
- 记忆写入错误可能持续影响后续 Agent，因此任务摘要应保留来源、时间、Agent 身份和验证结果。

## 回写建议

- 是否值得沉淀进 `wiki`：当前架构判断值得保留，但还需要一次真实三 Agent 联调后再正式升级。
- 建议沉淀到哪一页：后续可回写 [[Agent 框架设计]] 和 [[Agent 记忆与知识图谱]]；若形成稳定的接入步骤，再单独建立多 Agent 协作方法页。
