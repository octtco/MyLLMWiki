---
type: source
status: active
source_path: raw/repos/2026-04-14-github-lsdefine-genericagent/genericagent.md
source_type: repo
source_url: https://github.com/lsdefine/GenericAgent
source_bundle: raw/repos/2026-04-14-github-lsdefine-genericagent
title: GitHub - GenericAgent
authors:
  - lsdefine
created_at: 2026-04-22
updated_at: 2026-04-22
tags:
  - Agent
  - Framework
  - Memory
  - Skill
related_concepts:
  - 自进化 Agent
  - Skill
related_topics:
  - Agent 框架设计
related_relations: []
---

# GitHub - GenericAgent

## 一句话总结

这份 README 把 GenericAgent 定义成一种极简但会持续沉淀能力的 agent 框架：核心卖点不是工具很多，而是“少工具 + 分层记忆 + 任务后固化 skill”。

## 摘要

- README 把项目主张收成三块：`Layered Memory System`、`Autonomous Execution Loop`、`Minimal Toolset`。
- 它最突出的设计口径是 `don't preload skills — evolve them`，也就是把新任务完成路径沉淀成后续可复用的 skill。
- 当前最稳的知识抽取点，是它把长期能力积累问题直接拉到了 agent 框架中心。

## 证据或原文线索

- Overview 段落直接写出 `minimal, self-evolving autonomous agent framework` 和 `don't preload skills — evolve them`。
- `Layered Memory System` 把 L0 到 L4 的记忆层次列得很清楚，其中 L3 是 `Task Skills / SOPs`。
- `Minimal Toolset` 段落把 9 个原子工具列成核心能力底座。

## 我的判断

- 这份来源足够支撑 [[自进化 Agent]] 作为正式概念页。
- 它也能为 [[Skill]] 提供一条不同于 Trellis 的支持路径：不是规范协同，而是任务后沉淀能力。
- 但 README 里的比较表和 `Self-Bootstrap Proof` 仍然属于项目自述，不适合直接写成已独立验证结论。

## 相关概念

- [[自进化 Agent]]
- [[Skill]]

## 相关主题

- [[Agent 框架设计]]

## 关系

- `定义` -> [[自进化 Agent]]：README 对“任务后沉淀 skill/SOP”的说明最稳定。
- `支持` -> [[Skill]]：这份来源把 skill 明确放进长期能力累积机制里。
- `支持` -> [[Agent 框架设计]]：它提供了当前库里一条“少工具、重沉淀”的框架样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-04-14-github-lsdefine-genericagent/genericagent.md](../../raw/repos/2026-04-14-github-lsdefine-genericagent/genericagent.md)
