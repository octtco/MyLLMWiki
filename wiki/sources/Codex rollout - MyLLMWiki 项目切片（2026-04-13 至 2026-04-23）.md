---
type: source
source_type: chat
status: active
source_path: raw/chats/2026-04-13-to-2026-04-23-codex-rollout-myllmwiki-slice/inventory.md
source_bundle: raw/chats/2026-04-13-to-2026-04-23-codex-rollout-myllmwiki-slice
source_channel: codex rollout jsonl archive slice
title: Codex rollout - MyLLMWiki 项目切片（2026-04-13 至 2026-04-23）
participants:
  - liuyifu
  - Codex
time_range:
  start: 2026-04-13
  end: 2026-04-23
privacy: private
quote_policy: restricted
created_at: 2026-04-28
updated_at: 2026-04-29
tags:
  - 聊天归档
  - Codex
  - rollout
  - MyLLMWiki
  - 项目切片
related_entities:
  - MyLLMWiki
related_goals:
  - 把 MyLLMWiki 跑成可持续增长的个人 LLM Wiki
related_topics: []
related_methods: []
related_concepts: []
related_cases:
  - MyLLMWiki 分层知识库演化案例
---

# Codex rollout - MyLLMWiki 项目切片（2026-04-13 至 2026-04-23）

## 这次聊天在说什么

这不是一批杂聊天里的随便一段，而是从 Codex rollout 总归档里专门切出来的 `MyLLMWiki` 项目线。它集中记录了这座知识库从“我想做个人 LLM Wiki”一路长到“有 skill、有分层、有控制面、有对象页和目标页”的那段过程。

## 关键推进

- 最开始聊的是外部启发、KG / PARA / IRK 这些参照，但很快就落成了这座仓库自己的问题：`raw` 怎么只读、图片怎么归档、来源页先写什么。
- 后面不是只讲结构，而是一直拿真实来源来压测：先跑 Trellis / GenericAgent，再用《工程控制论》验证 longform 工作流，再把灵感、小工具和聊天历史接进 `Clippings / seeds / raw/chats / todo` 这套新版路径。
- 用户对主题页、方法页、概念页写法的连续反馈，也主要集中在这组会话里，于是方法页的“卡点 / 错法 / 这一步在做什么 / 最小动作 / 案例”结构，以及主题页“正文自然调用方法”的规则，才真正长稳。
- 这轮还顺手证明了一件事：`MyLLMWiki` 本身已经不只是一个目录，它已经是一个需要单独维护当前状态和目标推进的具体对象。

## 稳定信息

- `MyLLMWiki` 这条线最稳定的方法，不是先定一套完美知识架构，而是让真实材料不断把结构压出来，再把稳定部分写回 `skill`、`wiki/`、`todo/` 和 `_index/`。
- 长材料要先走 `outputs/` 工作层，这条规则不是空口定义，而是在《工程控制论》这条长文链里反复被验证出来的。
- 混合材料不能为了看起来整齐就硬塞成正式来源或概念页，`Clippings` 和 `seeds` 在这条项目线里是必要缓冲层。
- 当仓库自己已经成了被持续推进的对象时，`wiki/entities/` 和 `todo/goals/` 就不再只是模板占位，而是必须真的上场。

## 暂时还不能抽象的部分

- 这里面很多措辞微调、页面审美判断和 v0.x 规则讨论，仍然强依赖这座库的具体语境，不适合直接冒充通用方法论。
- 同一会话里也常常混着临时执行、试写、返工和偏好修正，所以不能跳过正式回写层，直接把聊天当最终结论。

## 建议回写

- 更新哪些对象页：[[MyLLMWiki]]，因为这份切片已经能更清楚地说明它是怎么从“知识库想法”变成“被持续维护的项目对象”的。
- 更新哪些目标页：[[把 MyLLMWiki 跑成可持续增长的个人 LLM Wiki]]，因为这份切片证明“按项目切分 rollout 聊天归档”已经跑出了第一份真实样板。
- 新增哪些待办：当前不必再为 `MyLLMWiki` 重复建同类任务；如果继续扩展这条线，下一步更适合只围绕 `WeBox` / `WhatsBox` 继续切小。
- 是否值得抽主题 / 方法 / 概念：这份切片本身不直接再抽新页，它更适合作为对象页、目标页和总归档来源页的补充语境。

## 关系

- `切片自` -> [[Codex rollout 历史聊天归档（2026-02 至 2026-04）]]：这是从总归档里切出来的第一份项目级子归档。
- `补充` -> [[MyLLMWiki]]：它把项目本体是怎么一步步长出结构和控制面的过程补得更清楚了。
- `支撑` -> [[把 MyLLMWiki 跑成可持续增长的个人 LLM Wiki]]：它直接证明这条目标里关于“对象页 / 目标页 / 聊天切片样板”的那部分已经开始落地。
- `支撑` -> [[MyLLMWiki 分层知识库演化案例]]：提供该案例的主要过程证据。

## 原始位置

- 对应原始文件：`raw/chats/2026-04-13-to-2026-04-23-codex-rollout-myllmwiki-slice/`
- 切片说明文件：[raw/chats/2026-04-13-to-2026-04-23-codex-rollout-myllmwiki-slice/inventory.md](../../raw/chats/2026-04-13-to-2026-04-23-codex-rollout-myllmwiki-slice/inventory.md)
