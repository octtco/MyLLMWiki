---
type: source
status: active
source_path: raw/repos/2026-06-02-github-tauricresearch-tradingagents/tradingagents.md
source_type: repo
source_url: https://github.com/TauricResearch/TradingAgents
source_bundle: raw/repos/2026-06-02-github-tauricresearch-tradingagents
title: GitHub - TradingAgents
authors:
  - TauricResearch
created_at: 2026-06-02
updated_at: 2026-06-02
tags:
  - Finance
  - Agent
  - Trading
  - Review
related_methods: []
related_concepts: []
related_topics:
  - AI 金融研究工具
  - Agent 框架设计
related_cases: []
related_relations: []
---

# GitHub - TradingAgents

## 一句话总结

TradingAgents 是一个多代理 LLM 金融交易研究框架，用 analyst、researcher、trader、risk management 和 portfolio manager 等角色模拟交易公司式决策流程。

## 当前范围

本页只整理 README 和 GitHub 元数据；不运行交易流程、不提供 ticker 建议、不把输出当作投资、交易或金融建议。

## 摘要

- README 明确把 TradingAgents 描述为 multi-agent trading framework，并把复杂交易任务拆成基本面、情绪、新闻、技术分析、研究辩论、交易员、风险管理和组合管理等角色。
- README 说明框架基于 LangGraph，并支持 OpenAI、Google、Anthropic、xAI、DeepSeek、Qwen、GLM、MiniMax、OpenRouter、Ollama、Azure OpenAI 等 provider。
- 项目提供 CLI 和 Python package 用法，也提到 Docker、LangGraph checkpoint resume、persistent decision log、structured-output agents 等更新。
- README 中直接声明该框架用于研究目的，不构成金融、投资或交易建议。

## 证据或原文线索

- GitHub API 抓取时显示 Apache-2.0 license，stars 约 81.8k，仓库未归档。
- GitHub 描述为 “TradingAgents: Multi-Agents LLM Financial Trading Framework”。
- README 指向 arXiv `2412.20138` 和项目方 disclaimer。

## 当前可支持的判断

- 当前来源支持：TradingAgents 是金融研究场景里多 agent 角色分工和辩论式决策编排的样本。
- 当前可保守迁出：它可以和 [[GitHub - AI Hedge Fund]] 一起支撑 [[AI 金融研究工具]]，但只能作为研究工具和框架样本保存。

## 当前边界

- 不提供投资建议，不写具体股票、交易方向或仓位建议。
- README 中的性能、版本和 provider 支持仍需按代码和真实运行环境复核。
- agent 决策、回测或模拟交易输出都不能视为收益证明。

## 相关主题

- [[AI 金融研究工具]]
- [[Agent 框架设计]]

## 关系

- `支持` -> [[AI 金融研究工具]]：提供多代理金融研究与模拟交易框架样本。
- `补充` -> [[Agent 框架设计]]：提供在金融场景下按角色、辩论和风险管理组织 agent 的样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-02-github-tauricresearch-tradingagents/tradingagents.md](../../raw/repos/2026-06-02-github-tauricresearch-tradingagents/tradingagents.md)
