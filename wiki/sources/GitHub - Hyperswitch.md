---
type: source
status: review
source_path: raw/repos/2026-05-29-github-juspay-hyperswitch/hyperswitch.md
source_type: repo
source_url: https://github.com/juspay/hyperswitch
source_bundle: raw/repos/2026-05-29-github-juspay-hyperswitch
title: GitHub - Hyperswitch
authors:
  - juspay
created_at: 2026-05-29
updated_at: 2026-05-29
tags:
  - Payments
  - Infrastructure
  - Rust
related_methods: []
related_concepts: []
related_topics: []
related_cases: []
related_relations: []
---

# GitHub - Hyperswitch

## 一句话总结

Hyperswitch 是 Juspay 开源的组合式支付基础设施，README 把它定位为可自托管、可模块化接入、面向多支付处理器连接和路由的 payments stack。

## 当前范围

本页只整理 README 与仓库元数据，不部署本地环境，不测试支付连接器，不评估 PCI 合规细节。

## 摘要

- README 标题把 Hyperswitch 定位为 composable open-source payments infrastructure。
- 它提供模块化支付能力，包括 cost observability、revenue recovery、vault、intelligent routing、reconciliation 和 alternate payment methods。
- README 提供 Docker 本地 quickstart、hosted sandbox 和云部署路径。
- 项目强调 Rust app server、支付路由、重试、vaulting、observability，以及 Control Center 中的可视化 workflow builder。
- Ecosystem mapping 把核心后端、dashboard、web checkout SDK、mobile SDK 和 deployment infrastructure 分成不同仓库与角色。

## 证据或原文线索

- GitHub API 抓取时显示 Apache-2.0 license，stars 约 42.8k，仓库未归档。
- README heading 包括 `What Can I Do with Hyperswitch?`、`Quickstart`、`Why Hyperswitch?`、`Supported Connectors`、`Hyperswitch Ecosystem Mapping`。
- 仓库 homepage 指向 `https://hyperswitch.io/`。

## 当前可支持的判断

- 当前来源支持：Hyperswitch 是开源支付基础设施方向的重要样本，尤其适合观察多 PSP 路由、vault、对账和支付可观测性如何被平台化。
- 当前可保守迁出：支付系统的复杂度不只是接一个 gateway，而是连接器、风控、重试、对账、密钥和合规边界共同构成的基础设施问题。

## 当前边界

- 不提供支付接入建议、合规建议或生产部署建议。
- README 中的 PCI、连接器数量和企业使用口径未实测。
- 当前库里支付基础设施来源还少，先不单独新建支付主题页。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-29-github-juspay-hyperswitch/hyperswitch.md](../../raw/repos/2026-05-29-github-juspay-hyperswitch/hyperswitch.md)

