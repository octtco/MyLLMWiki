---
type: source
status: active
source_path: raw/repos/2026-06-09-github-mvanhorn-last30days-skill/last30days-skill.md
source_type: repo
source_url: https://github.com/mvanhorn/last30days-skill
source_bundle: raw/repos/2026-06-09-github-mvanhorn-last30days-skill
title: GitHub - last30days-skill
authors:
  - mvanhorn
created_at: 2026-06-09
updated_at: 2026-06-09
tags:
  - Agent
  - Research
  - Skill
  - Review
related_methods: []
related_concepts:
  - Skill
related_topics:
  - AI 工具化知识工作流
  - Agent 框架设计
related_cases: []
related_relations: []
---

# GitHub - last30days-skill

## 一句话总结

last30days-skill 是一个面向 agent host 的近期互联网研究 skill，用 Reddit、X、YouTube、HN、Polymarket、GitHub 和网页等来源生成最近 30 天的 grounded brief。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未安装 skill，未测试各平台抓取、登录态、HTML brief、智能搜索、cluster merging 或 person-mode。

## 摘要

- README 把它定位为 `/last30days` agent skill，用于研究任意主题最近 30 天在多平台上的讨论和变化。
- README 强调 sources scored by people、shareable HTML briefs、intelligent search、Best Takes、cross-source cluster merging、single-pass comparisons、competitor comparisons、GitHub person-mode 和 ELI5 mode。
- 安装入口覆盖 Claude Code、Codex、Cursor、Copilot、Gemini CLI 等 Agent Skills hosts。
- GitHub API 抓取时显示 Python 仓库，MIT license，stars 约 34842，仓库未归档。

## 当前可支持的判断

- 当前来源支持：它是“近期信息研究”被封装成 agent skill 的样本。
- 当前可保守迁出：它补充 [[AI 工具化知识工作流]] 中“研究任务从一次性搜索变成可安装 skill / brief generator”的方向。
- 它也补充 [[Agent 框架设计]]：agent 的外部感知层可以被拆成可调用研究 skill，而不是写死在 host 内。

## 当前边界

- 多平台抓取、排序和聚类质量未实测。
- X、Reddit、YouTube、Polymarket 等来源可能涉及登录态、平台条款、限流和引用边界。
- 当前不把它写成事实核查工具或投资/舆情结论来源，只按研究 skill 样本保存。

## 相关主题

- [[AI 工具化知识工作流]]
- [[Agent 框架设计]]

## 关系

- `补充` -> [[AI 工具化知识工作流]]：提供本来源在该主题下的主要样本。
- `轻量补充` -> [[Agent 框架设计]]：提供相邻问题的补充样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-09-github-mvanhorn-last30days-skill/last30days-skill.md](../../raw/repos/2026-06-09-github-mvanhorn-last30days-skill/last30days-skill.md)
