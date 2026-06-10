---
type: source
status: active
source_path: raw/repos/2026-05-29-github-getzep-graphiti/graphiti.md
source_type: repo
source_url: https://github.com/getzep/graphiti
source_bundle: raw/repos/2026-05-29-github-getzep-graphiti
title: GitHub - Graphiti
authors:
  - getzep
created_at: 2026-05-29
updated_at: 2026-05-29
tags:
  - Agent Memory
  - Knowledge Graph
  - Retrieval
related_methods: []
related_concepts:
  - 可观测性
related_topics:
  - Agent 框架设计
  - AI 工具化知识工作流
  - Agent 记忆与知识图谱
related_cases: []
related_relations: []
---

# GitHub - Graphiti

## 一句话总结

Graphiti 是 GetZep 开源的 temporal context graph engine，用来为 AI agents 构建可随交互和数据变化增量更新的上下文图谱。

## 当前范围

本页只整理 README，不运行 Neo4j / FalkorDB / Kuzu / Neptune 后端，不验证检索延迟，也不复核 Zep 论文实验。

## 摘要

- README 把 Graphiti 定位为 building and querying temporal context graphs for AI agents 的框架。
- 它和静态知识图谱的区别在于：事实有时间有效窗口，关系变化会保留历史，派生事实可以回溯到 episodes 原始数据。
- Graphiti 支持从结构化和非结构化数据中构建图，支持 prescribed ontology 和 learned ontology。
- README 强调 incremental graph construction、hybrid retrieval、temporal fact management 和 provenance。
- 项目还提供 MCP server，让 Claude、Cursor 等 MCP clients 可以使用 context graph-based memory。
- README 明确区分 Zep 与 Graphiti：Zep 是托管上下文图基础设施，Graphiti 是开源 temporal context graph engine。

## 证据或原文线索

- GitHub API 抓取时显示 Apache-2.0 license，stars 约 26.7k，仓库未归档。
- README heading 包括 `What is a Context Graph?`、`Graphiti and Zep`、`Zep vs Graphiti`、`Why Graphiti?`、`Graphiti vs. GraphRAG`、`MCP Server`。
- 仓库 homepage 指向 `https://help.getzep.com/graphiti`。

## 当前可支持的判断

- 当前来源支持：Graphiti 代表 agent memory 从“聊天历史 / 文档 chunk”走向 temporal context graph 的路线。
- 当前可保守迁出：对长期运行的 agent 来说，记忆不只要存下来，还要能处理事实变化、来源回溯和按时间查询。

## 当前边界

- README 对 GraphRAG 和性能的比较未复测。
- 不把它写成所有 agent 记忆问题的默认解。
- Graphiti 默认依赖 LLM provider 和图数据库后端，实际部署成本仍需另行评估。

## 相关概念

- [[可观测性]]

## 相关主题

- [[Agent 框架设计]]
- [[AI 工具化知识工作流]]
- [[Agent 记忆与知识图谱]]

## 关系

- `支持` -> [[Agent 记忆与知识图谱]]：提供 temporal context graph 样本。
- `补充` -> [[Agent 框架设计]]：把 agent 的长期上下文层从 skill / SOP 扩到时间感知图谱。
- `补充` -> [[AI 工具化知识工作流]]：提供 MCP memory 和检索基础设施样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-29-github-getzep-graphiti/graphiti.md](../../raw/repos/2026-05-29-github-getzep-graphiti/graphiti.md)

