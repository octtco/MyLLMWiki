---
type: source
status: active
source_path: raw/web/2026-05-19-sakana-trinity/trinity.md
source_type: web
source_url: https://sakana.ai/trinity/
source_bundle: raw/web/2026-05-19-sakana-trinity
title: Sakana AI - Trinity: An Evolved LLM Coordinator
authors:
  - Sakana AI
created_at: 2026-05-19
updated_at: 2026-05-19
tags:
  - Agent
  - Framework
  - Coordinator
  - Multi-Model
related_methods: []
related_concepts: []
related_topics:
  - Agent 框架设计
related_cases: []
related_relations: []
---

# Sakana AI - Trinity: An Evolved LLM Coordinator

## 一句话总结

TRINITY 这页最值得保留的，是它把 agent 框架的设计抓手从“单个模型多会做事”推进到了“协调器怎样调度多个模型”。

## 当前范围

本页只整理 Sakana AI 这篇官方项目页，不补论文细节、独立复现或第三方评测。

## 摘要

- 页面把 TRINITY 明确写成 evolved LLM coordinator。
- 核心关注点不是单模型性能，而是协调器怎样安排多个角色与多个模型。
- 页面里的过程语义包含分工、批评、修正和整合，不是简单的并行调用。
- 这让当前知识库里的 [[Agent 框架设计]] 可以多出一条“协调器路线”。

## 证据或原文线索

- 官方页标题：`Trinity: An Evolved LLM Coordinator`
- 页面主定位直接落在 coordinator，而不是单独的 coding agent。
- 页面角色结构强调 Thinker / Worker / Verifier 一类分工。

## 当前可支持的判断

- 当前来源支持：agent 框架可以把“协调不同模型与角色”当成独立设计层，而不只是把多个 agent 并排摆放。
- 当前可保守迁出：多模型动态编排是一条值得单独观察的框架路线。

## 当前边界

- 当前主要仍是项目方材料，不适合直接写成“协调器路线已经证明优于其他框架”。
- 页面能支持“方向存在”，但还不够支持跨场景稳定泛化结论。

## 相关主题

- [[Agent 框架设计]]

## 关系

- `支持` -> [[Agent 框架设计]]：补强“协调器 / 动态编排”这条新路线。

## 回链

- 对应来源包主文件：[raw/web/2026-05-19-sakana-trinity/trinity.md](../../raw/web/2026-05-19-sakana-trinity/trinity.md)
