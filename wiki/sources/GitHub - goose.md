---
type: source
status: active
source_path: raw/repos/2026-06-08-github-aaif-goose-goose/goose.md
source_type: repo
source_url: https://github.com/aaif-goose/goose
source_bundle: raw/repos/2026-06-08-github-aaif-goose-goose
title: GitHub - goose
authors:
  - aaif-goose
created_at: 2026-06-08
updated_at: 2026-06-08
tags:
  - Agent
  - AI Coding
  - MCP
  - Review
related_methods: []
related_concepts: []
related_topics:
  - Agent 框架设计
  - AI coding framework
related_cases: []
related_relations: []
---

# GitHub - goose

## 一句话总结

goose 是 AAIF / Linux Foundation 旗下的本地开源 AI agent，提供桌面应用、CLI 和 API，支持代码、研究、写作、自动化、数据分析和 MCP extensions。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未安装桌面版或 CLI，未测试 provider、ACP、MCP extensions、文件编辑、执行或 API 嵌入。

## 摘要

- README 说明 goose 已从 `block/goose` 迁到 Agentic AI Foundation。
- goose 被描述为 general-purpose AI agent，运行在本地机器上，不只用于代码。
- README 提到 macOS、Linux、Windows desktop app、terminal CLI、API、Rust 实现、15+ providers 和 70+ MCP extensions。
- GitHub API 抓取时显示 Rust 仓库，Apache-2.0 license，stars 约 47544，仓库未归档。

## 当前可支持的判断

- 当前来源支持：goose 是本地 agent host / AI coding and workflow agent 样本。
- 当前可保守迁出：它补充 [[Agent 框架设计]] 中“agent 被放进 desktop / CLI / API 本地运行面”的路线。
- 它也补充 [[AI coding framework]] 中“编码之外的本地环境操作和扩展生态”这一侧。

## 当前边界

- README 的 provider 覆盖、ACP、MCP extensions 和本地执行能力需要实际安装验证。
- 本地 agent 能执行、编辑和自动化任务，后续测试要先确认文件权限、shell 权限和外部服务凭据边界。
- 当前不判断 goose 与 Codex、Claude Code、OpenCode 等 host 的优劣。

## 相关主题

- [[Agent 框架设计]]
- [[AI coding framework]]

## 回链

- 对应来源包主文件：[raw/repos/2026-06-08-github-aaif-goose-goose/goose.md](../../raw/repos/2026-06-08-github-aaif-goose-goose/goose.md)
