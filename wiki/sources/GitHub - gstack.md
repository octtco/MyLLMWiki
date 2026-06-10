---
type: source
status: active
source_path: raw/repos/2026-06-05-github-garrytan-gstack/gstack.md
source_type: repo
source_url: https://github.com/garrytan/gstack
source_bundle: raw/repos/2026-06-05-github-garrytan-gstack
title: GitHub - gstack
authors:
  - garrytan
created_at: 2026-06-05
updated_at: 2026-06-05
tags:
  - Agent
  - AI Coding
  - Workflow
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

# GitHub - gstack

## 一句话总结

gstack 是 Garry Tan 公开的一套 Claude Code / 多 host skill stack，把 AI coding 工作流组织成 CEO、设计、工程管理、代码审查、QA、安全、发布和文档等角色协作。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未安装 gstack，未验证 setup、team mode、浏览器、iOS QA、部署、security audit 或多 host 迁移行为。

## 摘要

- README 把 gstack 定位为 open source software factory，核心说法是把 Claude Code 变成一个 virtual engineering team。
- 它按 `Think -> Plan -> Build -> Review -> Test -> Ship -> Reflect` 组织流程，强调每个 skill 的产物会喂给下一步。
- README 列出 23 个 specialist 和 8 个 power tools，覆盖 `/office-hours`、计划审查、设计审查、代码审查、QA、security、发布、文档、retro、browser、spec 和 learn 等命令。
- 它不是只面向 Claude Code；README 还列出 Codex CLI、OpenCode、Cursor、Factory Droid、Slate、Kiro、Hermes、GBrain、OpenClaw 等 host 的安装目标。
- 项目还提供 `/careful`、`/freeze`、`/guard`、`/unfreeze` 这类安全 / 约束工具，以及浏览器、cookie、iOS QA、deploy、canary、benchmark 等更靠近真实交付面的工具入口。

## 证据或原文线索

- GitHub API 抓取时显示 MIT license，stars 约 107147，仓库未归档。
- GitHub 描述为 “Use Garry Tan's exact Claude Code setup: 23 opinionated tools that serve as CEO, Designer, Eng Manager, Release Manager, Doc Engineer, and QA”。
- README 明确把目标用户写成 founders / CEOs、first-time Claude Code users 和 tech leads / staff engineers。

## 当前可支持的判断

- 当前来源支持：gstack 是一个 AI coding agent 的角色化 workflow / skill stack 样本，而不是单一 prompt 库。
- 当前可保守迁出：它把 [[AI coding framework]] 里的 `Skill`、任务进入、审查、浏览器 QA、发布和文档回路放进同一套顺序流程里。
- 当前可保守迁出：它也补充 [[Agent 框架设计]] 的多角色路线，但更像“围绕一个 AI coding host 的虚拟工程团队”，不是从零实现的 agent runtime。

## 当前边界

- README 里的生产力倍数、贡献数和 “open source software factory” 属于项目方自述，当前不当作独立验证结论。
- 安装脚本、team mode 自动更新、浏览器、cookie、iOS QA、deploy、canary、benchmark 和 security audit 都需要隔离环境测试后再作为推荐。
- 多 host 支持当前只按 README 记录，未验证 Codex / OpenCode / Cursor 等环境里的实际 skill discovery 和冲突成本。
- 它的全局规则、hooks、浏览器代理和团队模式可能影响现有 Codex / Claude 配置，后续测试要先看可撤销性和最小安装面。

## 相关主题

- [[AI coding framework]]
- [[Agent 框架设计]]

## 关系

- `补充` -> [[AI coding framework]]：提供角色化 skill stack、审查、QA、发布和文档闭环样本。
- `补充` -> [[Agent 框架设计]]：提供 CEO / 设计 / 工程 / QA / 发布等多角色协作路线样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-05-github-garrytan-gstack/gstack.md](../../raw/repos/2026-06-05-github-garrytan-gstack/gstack.md)
