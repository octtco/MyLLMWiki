---
type: source
status: review
source_path: raw/repos/2026-06-02-github-everyinc-compound-engineering-plugin/compound-engineering-plugin.md
source_type: repo
source_url: https://github.com/EveryInc/compound-engineering-plugin
source_bundle: raw/repos/2026-06-02-github-everyinc-compound-engineering-plugin
title: GitHub - Compound Engineering
authors:
  - EveryInc
created_at: 2026-06-02
updated_at: 2026-06-02
tags:
  - Agent
  - Skill
  - Engineering Workflow
  - Review
related_methods: []
related_concepts:
  - Skill
related_topics:
  - AI coding framework
  - AI 工具化知识工作流
  - Agent 框架设计
related_cases: []
related_relations: []
---

# GitHub - Compound Engineering

## 一句话总结

Compound Engineering 是 EveryInc 发布的一套工程协作 plugin，把 strategy、ideation、brainstorm、planning、work、debug、review 和 compound note 组织成可安装的 agent / skill 工作流。

## 当前范围

本页只整理 README 和 GitHub 元数据；未安装 plugin，未运行其中的 agent、skill 或工作树流程。

## 摘要

- README 的核心口径是 “each unit of engineering work should make subsequent units easier”，强调计划、评审和知识沉淀。
- 工作流包括 `/ce-strategy`、`/ce-ideate`、`/ce-brainstorm`、`/ce-plan`、`/ce-work`、`/ce-debug`、`/ce-code-review`、`/ce-compound`、`/ce-product-pulse`。
- README 说明该 plugin 当前包含 37 个 skills 和 51 个 agents，并支持 Claude Code、Cursor、Codex、Copilot CLI、OpenCode、Gemini、Kiro 等环境的安装或转换。
- 对 Codex 的安装说明特别区分 marketplace 注册、agent set 安装和 TUI plugin 安装，说明它不是单一 prompt 包。

## 证据或原文线索

- GitHub API 抓取时显示 MIT license，stars 约 19.1k，仓库未归档。
- GitHub 描述为 “Official Compound Engineering plugin for Claude Code, Codex, Cursor, and more”。

## 当前可支持的判断

- 当前来源支持：Compound Engineering 是 agent coding 工作流 plugin 化、可安装化的样本。
- 当前可保守迁出：它把工程工作拆成策略、需求澄清、计划、执行、调试、评审、沉淀这条闭环，适合补充 [[AI coding framework]] 和 [[AI 工具化知识工作流]]。

## 当前边界

- 不把 README 的流程哲学直接写成已验证的软件工程最优实践。
- 当前未跑通安装、agent 调用、代码评审质量或 `ce-product-pulse` 数据输入。
- 它和普通 prompt 库不同，但仍需要真实项目样本来判断维护成本、学习成本和输出稳定性。

## 相关主题

- [[AI coding framework]]
- [[AI 工具化知识工作流]]
- [[Agent 框架设计]]

## 关系

- `支持` -> [[AI coding framework]]：提供 strategy / brainstorm / plan / work / review / compound 的工程工作流样本。
- `补充` -> [[AI 工具化知识工作流]]：提供知识沉淀和工程协作 plugin 化样本。
- `补充` -> [[Agent 框架设计]]：提供 multi-agent / multi-skill 工程闭环的运行面样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-02-github-everyinc-compound-engineering-plugin/compound-engineering-plugin.md](../../raw/repos/2026-06-02-github-everyinc-compound-engineering-plugin/compound-engineering-plugin.md)
