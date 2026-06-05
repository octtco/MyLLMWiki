---
type: source
status: review
source_path: raw/repos/2026-06-01-github-supermemoryai-supermemory/supermemory.md
source_type: repo
source_url: https://github.com/supermemoryai/supermemory
source_bundle: raw/repos/2026-06-01-github-supermemoryai-supermemory
title: GitHub - Supermemory
authors:
  - supermemoryai
created_at: 2026-06-01
updated_at: 2026-06-01
tags:
  - Agent Memory
  - MCP
  - Context
related_methods: []
related_concepts:
  - 可观测性
related_topics:
  - Agent 记忆与知识图谱
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - Supermemory

## 一句话总结

Supermemory 是面向 AI 的 memory 和 context layer，README 把它同时定位为个人 / 公司 brain、MCP 记忆服务和开发者 API。

## 当前范围

本页只整理 README 和元数据，不接入 MCP，不验证 benchmark，也不处理个人数据和隐私合规配置。

## 摘要

- README 把 Supermemory 描述为 memory and context layer for AI。
- 它强调从对话中抽取事实、维护用户画像、处理知识更新和矛盾、忘记过期信息，并在合适时间提供上下文。
- 使用形态包括 app、browser extension、Claude Code / OpenCode / OpenClaw / Hermes plugins，以及 MCP server。
- 开发者侧提供 memory、RAG、user profiles、connectors 和 file processing API。
- README 提到 Google Drive、Gmail、Notion、OneDrive、GitHub 等 connectors，以及 PDF、图片 OCR、视频转写、code AST-aware chunking。

## 证据或原文线索

- GitHub API 抓取时显示 MIT license，stars 约 23.4k，仓库未归档。
- README heading 包括 `Use Supermemory`、`Give your AI memory`、`MCP - Quick install`、`Build with Supermemory (API)`、`Benchmarks`。
- 仓库 homepage 指向 `https://supermemory.ai/docs`。

## 当前可支持的判断

- 当前来源支持：Supermemory 是 agent memory / context stack 平台化的样本，和 [[GitHub - Graphiti]] 共同扩展了“agent 记忆层”的材料池。
- 当前可保守迁出：AI 记忆不只是向量检索，还包含用户画像、事实抽取、过期遗忘、连接器和 MCP 接入。

## 当前边界

- README 中的 benchmark 排名未复测。
- 个人记忆和连接器涉及隐私、权限和数据保留，实际使用前必须单独评估。
- 不把它写成默认推荐的个人记忆服务。

## 相关概念

- [[可观测性]]

## 相关主题

- [[Agent 记忆与知识图谱]]
- [[AI 工具化知识工作流]]

## 关系

- `支持` -> [[Agent 记忆与知识图谱]]：提供 AI memory / context layer 平台样本。
- `补充` -> [[AI 工具化知识工作流]]：提供 MCP 记忆、连接器和上下文 API 样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-01-github-supermemoryai-supermemory/supermemory.md](../../raw/repos/2026-06-01-github-supermemoryai-supermemory/supermemory.md)

