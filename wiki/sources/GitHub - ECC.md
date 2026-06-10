---
type: source
status: active
source_path: raw/repos/2026-06-03-github-affaan-m-ecc/ecc.md
source_type: repo
source_url: https://github.com/affaan-m/ECC
source_bundle: raw/repos/2026-06-03-github-affaan-m-ecc
title: GitHub - ECC
authors:
  - affaan-m
created_at: 2026-06-03
updated_at: 2026-06-03
tags:
  - Agent
  - Harness
  - Skill
  - Review
related_methods: []
related_concepts:
  - Skill
related_topics:
  - AI coding framework
  - Agent 框架设计
related_cases: []
related_relations: []
---

# GitHub - ECC

## 一句话总结

ECC 是一套 cross-harness agent workflow / operator system，试图把 skills、rules、hooks、memory、security scanning 和 research-first development 打包成跨 Codex、Claude Code、Cursor、OpenCode 等环境的工作层。

## 当前范围

本页只整理 README 与 GitHub 元数据；未安装 ECC、未运行 hooks、未验证 GitHub App、AgentShield 或 dashboard。

## 摘要

- README 把 ECC 定位为 harness-native operator system for agentic work，而不是单一配置包。
- 它强调 skills、instincts、memory optimization、continuous learning、security scanning、research-first development 和 cross-harness packaging。
- README 中 v2.0.0-rc.1 提到 public Hermes operator story、dashboard GUI、63 agents、249 skills、79 legacy command shims、ECC 2.0 alpha Rust control-plane 等内容。
- 项目明确覆盖 Codex、Claude Code、Cursor、OpenCode、Gemini、Zed、GitHub Copilot 等 harness。

## 证据或原文线索

- GitHub API 抓取时显示 MIT license，stars 约 204k，仓库未归档。
- GitHub 描述为 “The agent harness performance optimization system...”。
- [[GitHub - revfactory Harness]] README 也把 `affaan-m/ECC` 放在 L2 Cross-Harness Workflow 相邻层。

## 当前可支持的判断

- 当前来源支持：ECC 是 AI coding harness 生态里的跨环境工作流层样本。
- 当前可保守迁出：它补充了 [[AI coding framework]] 中 “框架不只是单一 IDE / 单一 agent，而是在跨 harness 迁移 skills、hooks、rules 和 memory” 这条线。

## 当前边界

- README 的规模、stars、内部测试和性能口径未独立复测。
- 不直接建议叠加安装多个 agent / hook 系统；这类工具很容易引入重复规则、权限和上下文噪声。
- security scanning、memory hooks、GitHub App、Pro billing 等功能需要单独验证。

## 相关主题

- [[AI coding framework]]
- [[Agent 框架设计]]

## 关系

- `补充` -> [[AI coding framework]]：提供跨 harness 的 skill / hook / memory / security 工作层样本。
- `补充` -> [[Agent 框架设计]]：提供 agent harness performance 和 operator workflow 方向样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-03-github-affaan-m-ecc/ecc.md](../../raw/repos/2026-06-03-github-affaan-m-ecc/ecc.md)
