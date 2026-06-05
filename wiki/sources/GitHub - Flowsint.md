---
type: source
status: review
source_path: raw/repos/2026-06-03-github-reconurge-flowsint/flowsint.md
source_type: repo
source_url: https://github.com/reconurge/flowsint
source_bundle: raw/repos/2026-06-03-github-reconurge-flowsint
title: GitHub - Flowsint
authors:
  - reconurge
created_at: 2026-06-03
updated_at: 2026-06-03
tags:
  - OSINT
  - Graph
  - Investigation
  - Review
related_methods: []
related_concepts: []
related_topics:
  - OSINT 与图谱化调查
related_cases: []
related_relations: []
---

# GitHub - Flowsint

## 一句话总结

Flowsint 是一个开源 OSINT 图谱探索工具，面向网络安全分析师和调查人员，用视觉 graph interface 和 enrichers 组织实体关系调查。

## 当前范围

本页只整理 README 和 GitHub 元数据；不运行侦察流程，不扩写个人信息搜集、漏洞利用、账号追踪或数据泄露查询步骤。

## 摘要

- README 把 Flowsint 定位为 open-source OSINT graph exploration tool，并强调 ethical investigation、transparency、verification。
- 它提供 domain、IP、ASN、CIDR、social media、organization、crypto、website、email、phone、individual、N8n connector 等 enrichers。
- 项目结构包含 flowsint-core、flowsint-types、flowsint-enrichers、flowsint-api、flowsint-app。
- README 提到本地 Docker / Make 运行，数据存储在用户机器上。

## 证据或原文线索

- GitHub API 抓取时显示 Apache-2.0 license，stars 约 4.5k，仓库未归档。
- GitHub 描述为 “A modern platform for visual, flexible, and extensible graph-based investigations. For cybersecurity analysts and investigators.”
- README 开头直接提示阅读 `ETHICS.md`。

## 当前可支持的判断

- 当前来源支持：Flowsint 是 OSINT 调查工具里 “实体 -> 关系 -> enrichers -> graph” 的样本。
- 当前可保守迁出：它可以支撑 [[OSINT 与图谱化调查]]，但只能在合法授权、伦理边界和隐私保护下讨论。

## 当前边界

- 不迁出具体个人搜索、泄露库查询、目标画像或绕限制操作。
- 不把 OSINT 工具默认写成可对任意个人或组织使用。
- README 的 enrichers 覆盖面和实际准确率未复测。

## 相关主题

- [[OSINT 与图谱化调查]]

## 关系

- `支持` -> [[OSINT 与图谱化调查]]：提供图谱化 OSINT 调查平台样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-03-github-reconurge-flowsint/flowsint.md](../../raw/repos/2026-06-03-github-reconurge-flowsint/flowsint.md)
