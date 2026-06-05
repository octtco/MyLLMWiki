---
type: source
status: review
source_path: raw/repos/2026-05-25-github-multica-ai-andrej-karpathy-skills/andrej-karpathy-skills.md
source_type: repo
source_url: https://github.com/multica-ai/andrej-karpathy-skills
source_bundle: raw/repos/2026-05-25-github-multica-ai-andrej-karpathy-skills
title: GitHub - andrej-karpathy-skills
authors:
  - multica-ai
created_at: 2026-05-25
updated_at: 2026-05-25
tags:
  - Claude Code
  - Skill
  - Coding Agent
related_methods: []
related_concepts:
  - Skill
  - 反默认输出
related_topics:
  - AI coding framework
related_cases: []
related_relations: []
---

# GitHub - andrej-karpathy-skills

## 一句话总结

andrej-karpathy-skills 是把 Karpathy 对 LLM coding 坑点的观察压进单个 `CLAUDE.md` 的规则文件样本，价值在于“行为约束如何变成可复制工程纪律”。

## 当前范围

本页只整理 README 入口，不判断它是否忠实代表 Karpathy 原意，也不直接替换当前仓库规则。

## 摘要

- README 把问题概括为：模型会擅自假设、过度复杂化、改动无关代码、偏离目标。
- 方案是用四个原则约束 Claude Code：think before coding、simplicity first、surgical changes、goal-driven execution。
- 它不是完整框架，更像一个高传播度规则文件。
- 对 [[AI coding framework]] 来说，它补的是“最小规则文件如何约束 coding agent 行为”的样本。

## 证据或原文线索

- GitHub API 抓取时显示 stars 约 152k，仓库未归档。
- README 标题为 `Karpathy-Inspired Claude Code Guidelines`，并提到项目派生自 Karpathy 对 LLM coding pitfalls 的观察。

## 当前可支持的判断

- 当前来源支持：coding agent 的质量问题可以通过规则文件显式约束，而不是只靠模型能力。
- 当前可保守迁出：单个 `CLAUDE.md` 可以承载轻量行为规范，但不等于完整任务系统。

## 当前边界

- stars 极高不等于规则普适有效。
- 需要区分“Karpathy-inspired”与 Karpathy 本人维护。

## 相关概念

- [[Skill]]
- [[反默认输出]]

## 相关主题

- [[AI coding framework]]

## 关系

- `补充` -> [[AI coding framework]]：提供单文件 coding-agent 行为规范样本。
- `相关` -> [[反默认输出]]：共同关心模型默认坏习惯的约束。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-25-github-multica-ai-andrej-karpathy-skills/andrej-karpathy-skills.md](../../raw/repos/2026-05-25-github-multica-ai-andrej-karpathy-skills/andrej-karpathy-skills.md)
