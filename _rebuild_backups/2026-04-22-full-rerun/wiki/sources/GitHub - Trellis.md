---
type: source
status: active
source_path: raw/repos/2026-04-14-github-mindfold-ai-trellis/trellis.md
source_type: repo_readme
source_url: https://github.com/mindfold-ai/Trellis
source_bundle: raw/repos/2026-04-14-github-mindfold-ai-trellis
title: Trellis
authors:
  - mindfold-ai
year: 2026
created_at: 2026-04-14
updated_at: 2026-04-14
temporal_status: evolving
confidence: medium
claim_status: mixed
tags:
  - Trellis
  - Agent Harness
  - AI Coding Framework
  - Spec
  - Task Workflow
  - Multi-platform
related_concepts:
  - Spec
  - Skill
  - Spec 注入
  - Task-centered workflow
  - Project memory
  - Multi-platform AI coding
related_topics:
  - AI coding framework
---

# Trellis

## 一句话总结

Trellis 是一个面向多平台 AI coding 工具的结构化工作流框架，核心卖点是把 spec、task、workspace memory 和平台接入统一到一套可复用目录结构里。

## 摘要

- 这是项目仓库 README 的一手来源，代表 Trellis 团队对产品定位和工作流的官方定义。
- README 把 Trellis 定位成 “multi-platform AI coding framework”，强调不是只服务单一工具，而是要在多种 AI coding 平台之间复用同一套工作流。
- 项目最核心的结构围绕 `.trellis/` 展开，主要包括 `spec/`、`tasks/`、`workspace/`、`workflow.md` 和 `scripts/`。
- README 强调自动注入 specs、任务中心工作流、并行 agent 执行、项目记忆和团队共享标准这五类能力。
- 初始化方式很轻，核心命令是 `npm install -g @mindfoldhq/trellis@latest` 和 `trellis init ...`。
- Trellis 同时支持多种平台接入，包括 Claude Code、Cursor、Codex、OpenCode、Copilot 等，这说明它更像“工作流层”而不是某个单独 agent 的实现。

## 关键点

- Trellis 的中心思想不是单纯加一个规则文件，而是把 AI coding 所需的规范、任务、记忆和平台接线都放进同一套 repo 结构。
- README 把 `spec` 和 `task` 都放在很核心的位置，这和只靠单一 `AGENTS.md` 或 `CLAUDE.md` 的做法不一样。
- 项目很强调跨工具一致性，意思是团队可以换不同 AI coding 工具，但底层工作流不用反复重搭。
- 它还把 git worktree 和并行 agent 当成默认能力的一部分，说明目标场景偏团队协作和多任务推进，而不是只服务单轮对话。

## 证据或原文线索

- README 标题下直接写明它是 “The best agent harness” 和 “A multi-platform AI coding framework”。
- README 明确列出支持的平台，包括 Claude Code、Cursor、Codex、OpenCode、Copilot 等。
- `Why Trellis?` 一节明确列出 `Auto-injected specs`、`Task-centered workflow`、`Parallel agent execution`、`Project memory`、`Team-shared standards`、`Multi-platform setup`。
- `How It Works` 一节给出 `.trellis/` 目录结构，并说明还会生成 `.claude/`、`.cursor/`、`AGENTS.md`、`.codex/` 等平台接入文件。
- `Quick Start` 一节给出安装和初始化命令，说明这个项目已经是可直接上手的工具，而不是概念草图。

## 可直接回证的能力或主张

- 多平台支持、`.trellis/` 目录结构、`spec/tasks/workspace` 三层组织、初始化命令，这些都属于 README 直接写明的能力。
- `Auto-injected specs`、`Task-centered workflow`、`Parallel agent execution`、`Project memory` 这些也属于 README 的明确产品功能叙事。
- Trellis 是“工作流层”而不是单一 agent 实现，这个判断也能从它支持多平台和生成多套接入文件的做法里得到支撑。

## 更偏项目方自述或待验证的判断

- `The best agent harness` 这类判断首先是品牌口号，不应直接当成客观结论。
- “更适合团队”“明显优于单规则文件”“几乎没有额外成本”这类效果判断，需要更多用户侧材料才能沉淀。
- README 虽然给出很多能力面，但具体效果、规模表现和迁移成本，仍需要更多外部证据。

## 我的判断

- 这是一篇应该保留为主来源的页面，后面如果要整理 Trellis 的概念页或主题页，都应该优先回链到这里。
- 目前可以相对稳地沉淀的是：Trellis 如何组织结构、如何接入多平台、如何把 spec/task/memory 组合成工作流。
- 不能直接当成已证实事实的，是 README 里的优势口号，比如 “best harness” 或“明显优于传统规则文件”的效果判断。
- 如果后面继续扩写，比较值得补的是 docs 里的平台接入细节和任务生命周期设计，而不是马上上升到大而全的主题综述。

## 相关概念

- Spec 注入
- Task-centered workflow
- Project memory
- Multi-platform AI coding

## 相关主题

- [[AI coding framework]]

## 关系

- `支持` -> [[Spec]]：README 明确把规范层放进稳定工作流结构里。
- `支持` -> [[Skill]]：README 也支撑能力层按需接入，而不是只靠静态规则。
- `支持` -> [[AI coding framework]]：它把 Trellis 明确定位成多平台 AI coding 的工作流层，而不是单一 agent 实现。
- `主说明` -> [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]：本页负责产品结构定义，论坛帖负责补设计动机与问题诊断。

## 回链

- 对应原始文件：[raw/repos/2026-04-14-github-mindfold-ai-trellis/trellis.md](../../raw/repos/2026-04-14-github-mindfold-ai-trellis/trellis.md)
- 对应外部来源：[GitHub - mindfold-ai/Trellis](https://github.com/mindfold-ai/Trellis)
