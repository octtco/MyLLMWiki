---
type: source
status: review
source_path: raw/repos/2026-06-04-github-ganyuanran-aegis/aegis.md
source_type: repo
source_url: https://github.com/GanyuanRan/Aegis
source_bundle: raw/repos/2026-06-04-github-ganyuanran-aegis
title: GitHub - Aegis
authors:
  - GanyuanRan
created_at: 2026-06-04
updated_at: 2026-06-04
tags:
  - Agent
  - Skill
  - Verification
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

# GitHub - Aegis

## 一句话总结

Aegis 是一套面向 AI coding agents 的 method pack，强调 baseline-first planning、evidence before completion claims、repair / retirement track 和按风险调节的 workflow quality。

## 当前范围

本页只整理 README 和 GitHub 元数据；未安装 Aegis，未运行 doctor、update、host discovery 或完整 workflow 验证。

## 摘要

- README 把 Aegis 定位为 “Baseline-first, evidence-driven workflow discipline for AI coding agents”。
- 它保留 composable skills 的思路，同时补 baseline-first planning、completion evidence、bug / fallback / compatibility path 的 repair plus retirement、workflow guardrails 和 portable method-pack skills。
- README 明确 Aegis 当前是 `runtime-ready method pack`，不是 full platform、daemon、runtime core、authoritative GateDecision、PolicySnapshot 或 final completion authority。
- 支持面覆盖 Codex、OpenCode、Claude Code、CodeBuddy、DeepSeek-TUI、Trae、GitHub Copilot、Qoder、CC GUI、Antigravity、Pi CLI、OpenClaw、Hermes Agent 等 host，但不同 host 的 smoke 状态不同。

## 证据或原文线索

- GitHub API 抓取时显示 MIT license，stars 约 436，仓库未归档。
- GitHub 描述为 “Make AI coding agents architecture-aware: baseline-first, evidence-verified, drift-checked, and safe across long tasks.”
- README 明确说 user instructions 和 target-project rules outrank Aegis guidance。

## 当前可支持的判断

- 当前来源支持：Aegis 是 AI coding agent 的方法纪律层，而不是独立 agent runtime。
- 当前可保守迁出：它补充 [[AI coding framework]] 中 “框架不只要组织能力，还要组织任务进入、证据验收和退役旧路径” 这一侧。

## 当前边界

- 不把 Aegis 写成最终完成判定器；README 自己也说明它不是 final completion authority。
- 当前未验证多 host 安装、skill discovery、activation mode、TDD routing 或 doctor JSON。
- 它的流程纪律需要和目标项目规则、用户指令、现有 Codex 全局规则一起判断，不能盲目叠加。

## 相关主题

- [[AI coding framework]]
- [[Agent 框架设计]]

## 关系

- `补充` -> [[AI coding framework]]：提供 baseline-first、evidence-driven、risk-routed workflow discipline 样本。
- `补充` -> [[Agent 框架设计]]：提供 method-pack 层对 agent 长任务和架构漂移的约束样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-04-github-ganyuanran-aegis/aegis.md](../../raw/repos/2026-06-04-github-ganyuanran-aegis/aegis.md)
