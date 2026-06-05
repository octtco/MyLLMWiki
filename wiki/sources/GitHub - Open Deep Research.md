---
type: source
status: review
source_path: raw/repos/2026-05-28-github-langchain-ai-open-deep-research/open-deep-research.md
source_type: repo
source_url: https://github.com/langchain-ai/open_deep_research
source_bundle: raw/repos/2026-05-28-github-langchain-ai-open-deep-research
title: GitHub - Open Deep Research
authors:
  - langchain-ai
created_at: 2026-05-28
updated_at: 2026-05-28
tags:
  - Agent
  - Deep Research
  - LangGraph
related_methods: []
related_concepts: []
related_topics:
  - Agent 框架设计
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - Open Deep Research

## 一句话总结

Open Deep Research 是 LangChain 开源的可配置 deep research agent 样本，强调跨模型、搜索工具和 MCP server 的研究流程编排。

## 当前范围

本页只整理 README，不启动 LangGraph server，不复测 Deep Research Bench，也不验证 leaderboard 排名。

## 摘要

- README 把 deep research 称为热门 agent application，并把本项目定位为 simple、configurable、fully open source deep research agent。
- 项目可配置多个 LLM 角色：summarization、research、compression、final report model。
- 搜索层默认使用 Tavily，同时提到 MCP compatibility、Anthropic / OpenAI native web search。
- 部署和使用形态包括本地 LangGraph Studio、LangGraph Platform 和 Open Agent Platform。
- README 公开了 Deep Research Bench 评估路径、成本提醒和部分结果表。
- `src/legacy/` 中保留 workflow implementation 和 multi-agent implementation，作为旧方案对照。

## 证据或原文线索

- GitHub API 抓取时显示 MIT license，stars 约 11.5k，仓库未归档。
- README heading 包括 `Quickstart`、`Configurations`、`Evaluation`、`Deployments and Usage`、`Legacy Implementations`。
- README 中对完整评估给出约 `$20-$100` 成本提醒。

## 当前可支持的判断

- 当前来源支持：deep research agent 可以拆成搜索、研究、压缩、报告生成和评估提交等多个可配置环节。
- 当前可保守迁出：研究型 agent 的成熟度不只看“能写报告”，还要看它是否有可复现配置和评估路径。

## 当前边界

- README 的 benchmark 排名和分数未复测，不能当作本库已确认性能。
- 不把它写成“深度研究最终形态”，当前只作为开放实现样本。

## 相关主题

- [[Agent 框架设计]]
- [[AI 工具化知识工作流]]

## 关系

- `支持` -> [[Agent 框架设计]]：提供 deep research agent 的 LangGraph 样本。
- `支持` -> [[AI 工具化知识工作流]]：把研究任务从聊天式问答推进到可配置、可评估、可部署的工作流。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-28-github-langchain-ai-open-deep-research/open-deep-research.md](../../raw/repos/2026-05-28-github-langchain-ai-open-deep-research/open-deep-research.md)

