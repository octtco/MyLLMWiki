---
type: source
status: active
source_path: raw/repos/2026-05-25-github-colbymchenry-codegraph/codegraph.md
source_type: repo
source_url: https://github.com/colbymchenry/codegraph
source_bundle: raw/repos/2026-05-25-github-colbymchenry-codegraph
title: GitHub - CodeGraph
authors:
  - colbymchenry
created_at: 2026-05-25
updated_at: 2026-05-25
tags:
  - Codebase Analysis
  - Knowledge Graph
  - AI Coding
related_methods: []
related_concepts:
  - 顺藤摸瓜式搜索
related_topics:
  - AI coding framework
  - 代码库图谱化理解
related_cases: []
related_relations: []
---

# GitHub - CodeGraph

## 一句话总结

CodeGraph 是给 Claude Code、Codex、Cursor 等 coding agent 使用的本地代码知识图谱样本，主张用预索引降低 token 和工具调用成本。

## 当前范围

本页只整理 README 入口，不安装 npm 包，不复测 benchmark。

## 摘要

- README 把 CodeGraph 定位为 semantic code intelligence layer。
- 项目强调 `100% local`、更少 tool calls、更低成本。
- 它面向 Claude Code、Cursor、Codex CLI、OpenCode、Hermes Agent 等工具。
- 对当前知识库来说，它和 [[GitHub - Understand Anything]] 共同支撑“代码库图谱化理解”这条线。

## 证据或原文线索

- GitHub API 抓取时显示 MIT license，stars 约 22.4k，仓库未归档。
- README heading 包括 `Why CodeGraph?`、`Benchmark Results`、`Key Features`、`Framework-aware Routes`。

## 当前可支持的判断

- 当前来源支持：为 agent 预建本地代码索引，是降低反复读文件和盲搜成本的一种路线。
- 当前可保守迁出：代码图谱更像检索 / 定位层，不等于自动证明修改正确。

## 当前边界

- README benchmark 口径未复测，不能直接写成稳定收益。
- 不评价它与 Understand Anything 谁更好。

## 相关概念

- [[顺藤摸瓜式搜索]]

## 相关主题

- [[AI coding framework]]
- [[代码库图谱化理解]]

## 关系

- `支持` -> [[代码库图谱化理解]]：提供本地预索引代码图谱样本。
- `补充` -> [[AI coding framework]]：把框架的上下文供给层从规则文件扩到图谱索引。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-25-github-colbymchenry-codegraph/codegraph.md](../../raw/repos/2026-05-25-github-colbymchenry-codegraph/codegraph.md)
