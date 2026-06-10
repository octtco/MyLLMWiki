---
type: source
status: active
source_path: raw/repos/2026-06-02-github-revfactory-harness/revfactory-harness.md
source_type: repo
source_url: https://github.com/revfactory/harness
source_bundle: raw/repos/2026-06-02-github-revfactory-harness
title: GitHub - revfactory Harness
authors:
  - revfactory
created_at: 2026-06-02
updated_at: 2026-06-02
tags:
  - Agent
  - Skill
  - Claude Code
  - Review
related_methods: []
related_concepts:
  - Skill
related_topics:
  - Agent 框架设计
  - AI coding framework
related_cases: []
related_relations: []
---

# GitHub - revfactory Harness

## 一句话总结

revfactory Harness 是一个面向 Claude Code 的 team-architecture factory，用项目领域描述生成 agent team 和对应 skills。

## 当前范围

本页只整理 README 和 GitHub 元数据；未安装 Claude Code plugin，未生成实际 `.claude/agents/` 或 `.claude/skills/`。

## 摘要

- README 把该项目定位为 “team-architecture factory”，触发语类似 “build a harness for this project”。
- 它声明基于 6 种 team architecture patterns：Pipeline、Fan-out/Fan-in、Expert Pool、Producer-Reviewer、Supervisor、Hierarchical Delegation。
- 产物包括 agent definitions 和 skills，目标是把领域描述转成具体 agent 团队结构。
- README 还把项目放在 Claude Code 生态的 L3 Meta-Factory / Team-Architecture Factory 层，并与 Archon、meta-harness、ECC 等相邻项目区分。

## 证据或原文线索

- GitHub API 抓取时显示 Apache-2.0 license，stars 约 5.2k，仓库未归档。
- GitHub 描述为 “A meta-skill that designs domain-specific agent teams, defines specialized agents, and generates the skills they use.”

## 当前可支持的判断

- 当前来源支持：revfactory Harness 是 agent team / skill 生成器，而不是普通 agent runtime。
- 当前可保守迁出：它补充了 [[Agent 框架设计]] 中 “框架生成框架” 或 meta-factory 方向的样本。

## 当前边界

- 不与已有 [[GitHub - Harness]] 混同；二者来源 URL、作者和项目定位不同。
- README 的层级分类属于项目方口径，当前只作为自我定位保存。
- 未验证生成出的 agent team 在真实任务中的质量、可维护性和安全边界。

## 相关主题

- [[Agent 框架设计]]
- [[AI coding framework]]

## 关系

- `补充` -> [[Agent 框架设计]]：提供由领域描述生成 agent team 和 skill 的 meta-factory 样本。
- `补充` -> [[AI coding framework]]：说明 coding agent 生态里出现了专门生成 team architecture 的 plugin。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-02-github-revfactory-harness/revfactory-harness.md](../../raw/repos/2026-06-02-github-revfactory-harness/revfactory-harness.md)
