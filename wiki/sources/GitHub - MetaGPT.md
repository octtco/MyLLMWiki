---
type: source
status: active
source_path: raw/repos/2026-05-15-github-foundationagents-metagpt/metagpt.md
source_type: repo
source_url: https://github.com/FoundationAgents/MetaGPT
source_bundle: raw/repos/2026-05-15-github-foundationagents-metagpt
title: GitHub - MetaGPT
authors:
  - FoundationAgents
created_at: 2026-05-15
updated_at: 2026-05-15
tags:
  - Agent
  - Framework
  - Multi-Agent
  - SOP
related_methods: []
related_concepts:
  - Skill
related_topics:
  - Agent 框架设计
  - AI coding framework
related_cases: []
related_relations: []
---

# GitHub - MetaGPT

## 一句话总结

MetaGPT 是一个软件公司式 multi-agent framework 样本：它最值得保留的不是“又一个会写代码的 agent”，而是把角色分工、SOP 和团队协作放进 agent 框架设计里。

## 当前范围

本页只整理仓库 README / 入口层信息，不分析完整代码实现、论文或 benchmark。

## 摘要

- MetaGPT 把 agent 组织成类似软件公司的多角色团队。
- 它用 SOP 来承接团队协作流程，典型口径是 `Code = SOP(Team)`。
- 这和 [[GitHub - GenericAgent]] 的“任务后沉淀 skill/SOP”不是同一条线：GenericAgent 更强调经验沉淀，MetaGPT 更强调角色分工和流程编排。
- 对当前知识库来说，它能补强 [[Agent 框架设计]] 中“框架如何组织多个角色共同完成软件任务”的部分。

## 证据或原文线索

- GitHub 仓库：`https://github.com/FoundationAgents/MetaGPT`
- README 以 multi-agent framework、software company、SOP / team 这类语义组织自身定位。

## 当前可支持的判断

- 当前来源支持：agent 框架可以把软件开发流程显式建模成角色团队和 SOP，而不是只靠单个 coding agent。
- 当前可保守迁出：当任务天然跨产品、架构、工程和测试等职责时，多角色流程编排是一个值得单独观察的框架抓手。

## 当前边界

- 不把 MetaGPT 写成“最强多智能体框架”。
- 不把角色分工本身等同于交付质量；真实效果仍要看任务、工具、上下文和验证流程。

## 相关概念

- [[Skill]]

## 相关主题

- [[Agent 框架设计]]
- [[AI coding framework]]

## 关系

- `支持` -> [[Agent 框架设计]]：提供软件公司式多角色 SOP 框架样本。
- `补充` -> [[AI coding framework]]：补足 Trellis / GenericAgent 之外的多角色框架路线。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-15-github-foundationagents-metagpt/metagpt.md](../../raw/repos/2026-05-15-github-foundationagents-metagpt/metagpt.md)
