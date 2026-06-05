---
type: source
status: review
source_path: raw/repos/2026-05-25-github-anthropics-knowledge-work-plugins/knowledge-work-plugins.md
source_type: repo
source_url: https://github.com/anthropics/knowledge-work-plugins
source_bundle: raw/repos/2026-05-25-github-anthropics-knowledge-work-plugins
title: GitHub - knowledge-work-plugins
authors:
  - Anthropic
created_at: 2026-05-25
updated_at: 2026-05-25
tags:
  - Claude
  - Plugin
  - Knowledge Work
related_methods: []
related_concepts:
  - Skill
related_topics:
  - AI coding framework
  - Agent 框架设计
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - knowledge-work-plugins

## 一句话总结

knowledge-work-plugins 是 Anthropic 面向知识工作者开源的 plugin 集合，最值得保留的是“角色 / 团队工作流如何打包成插件”的样本。

## 当前范围

本页只整理仓库 README 入口，不逐个插件拆解，也不验证 Claude Cowork 或 Claude Code 安装流程。

## 摘要

- README 把 plugins 定义为让 Claude 更像特定角色、团队和公司里的 specialist。
- plugin 可以包含 skills、connectors、slash commands、sub-agents。
- 仓库面向 Claude Cowork，同时兼容 Claude Code。
- README 强调插件可被团队定制成公司自己的工具、术语和流程。

## 证据或原文线索

- GitHub API 抓取时显示 Apache-2.0，stars 约 14.1k，仓库未归档。
- README heading 包括 `Why Plugins`、`Plugin Marketplace`、`How Plugins Work`、`Making Them Yours`。

## 当前可支持的判断

- 当前来源支持：知识工作中的 AI 能力可以被打包成 plugin，而不仅是一次性 prompt 或单个 skill。
- 当前可保守迁出：plugin 的价值在于把角色、连接器、命令和子代理组织成可复用工作面。

## 当前边界

- 不判断这 11 个插件的实际成熟度。
- Claude Cowork 产品和插件机制仍可能变化，先保持 `review`。

## 相关概念

- [[Skill]]

## 相关主题

- [[AI coding framework]]
- [[Agent 框架设计]]
- [[AI 工具化知识工作流]]

## 关系

- `支持` -> [[AI 工具化知识工作流]]：提供知识工作 plugin 市场样本。
- `补充` -> [[Agent 框架设计]]：把 skills、connectors、commands、sub-agents 组织到插件边界里。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-25-github-anthropics-knowledge-work-plugins/knowledge-work-plugins.md](../../raw/repos/2026-05-25-github-anthropics-knowledge-work-plugins/knowledge-work-plugins.md)
