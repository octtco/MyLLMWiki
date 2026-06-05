---
type: source
status: review
source_path: raw/repos/2026-06-02-github-pbakaus-impeccable/impeccable.md
source_type: repo
source_url: https://github.com/pbakaus/impeccable
source_bundle: raw/repos/2026-06-02-github-pbakaus-impeccable
title: GitHub - Impeccable
authors:
  - pbakaus
created_at: 2026-06-02
updated_at: 2026-06-02
tags:
  - Design
  - Skill
  - Frontend
  - Review
related_methods: []
related_concepts:
  - Skill
related_topics:
  - 设计系统与平台规范
  - AI coding framework
related_cases: []
related_relations: []
---

# GitHub - Impeccable

## 一句话总结

Impeccable 是一套面向 AI 前端设计的 skill / command / anti-pattern 组合，试图给 coding agent 补设计语言、视觉审查和前端体验打磨流程。

## 当前范围

本页只整理 README 和 GitHub 元数据；未安装 skill，未跑 CLI、浏览器扩展或视觉评测。

## 摘要

- README 把 Impeccable 定位成 “1 skill, 23 commands, curated anti-patterns”，核心目标是减少 AI 生成前端时常见的模板化设计痕迹。
- 它包含 typography、color-and-contrast、spatial design、motion、interaction、responsive、UX writing 等 7 个 reference 文件。
- 命令层覆盖 `craft`、`shape`、`critique`、`audit`、`polish`、`harden`、`animate`、`typeset`、`layout` 等前端设计和验收动作。
- README 提到 CLI installer 会按目标 harness 生成适配版本，支持 Claude Code、Cursor、Gemini CLI、Codex CLI 等环境。

## 证据或原文线索

- GitHub API 抓取时显示 Apache-2.0 license，stars 约 32.8k，仓库未归档。
- GitHub 描述为 “The design language that makes your AI harness better at design.”

## 当前可支持的判断

- 当前来源支持：Impeccable 可作为 “AI coding 环境里的设计 skill” 样本，而不是普通设计系统目录。
- 当前可保守迁出：它把设计判断拆成 reference、command 和 deterministic anti-pattern rule，适合补充 [[设计系统与平台规范]] 里 “平台规范之外的 agent 设计纪律” 这一侧。

## 当前边界

- 不把 README 里的效果展示当成普遍设计质量证明。
- 不把 anti-pattern 规则直接升级成通用审美标准；具体项目仍要看产品语境和用户群。
- 当前未验证安装流程、命令效果、浏览器扩展和跨 harness 兼容性。

## 相关主题

- [[设计系统与平台规范]]
- [[AI coding framework]]

## 关系

- `补充` -> [[设计系统与平台规范]]：提供 AI 前端生成场景下的设计 skill 和反模式清单样本。
- `补充` -> [[AI coding framework]]：说明 skill 可以承担设计审查和前端体验打磨这类专门能力。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-02-github-pbakaus-impeccable/impeccable.md](../../raw/repos/2026-06-02-github-pbakaus-impeccable/impeccable.md)
