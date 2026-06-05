---
type: topic
status: review
tags:
  - OSINT
  - Graph
  - Investigation
related_topics:
  - 信息源订阅与内容聚合
related_methods: []
related_concepts: []
related_relations: []
source_pages:
  - GitHub - Flowsint
updated: 2026-06-03
---

# OSINT 与图谱化调查

## 这页真正想回答什么

这页先收一个窄问题：OSINT 工具什么时候不是简单搜索入口，而是把实体、关系和证据组织成调查图谱。

## 当前最稳的主线

[[GitHub - Flowsint]] 当前提供的样本是：把 domain、IP、ASN、organization、website、email、phone、crypto wallet、social profile 等对象统一成 typed entities，再用 enrichers 把关系扩出来，最后在 graph interface 中检查和验证。

这条线和普通信息源聚合不同。RSS 或网页抓取关心的是“信息怎么进入系统”，OSINT 图谱调查更关心“实体之间是什么关系、证据从哪里来、能不能被复核”。所以它暂时独立成页，不塞进 [[信息源订阅与内容聚合]]。

## 当前边界

- 当前只有 Flowsint 一个来源，先不扩成 OSINT 方法论。
- 不迁出针对个人、账号、泄露库或组织目标的操作步骤。
- OSINT 必须受合法授权、隐私保护、平台条款和伦理边界约束。

## 代表性来源

- [[GitHub - Flowsint]]

## 关系

- `支持` <- [[GitHub - Flowsint]]：提供图谱化 OSINT 调查工具样本。

## 相关主题

- [[信息源订阅与内容聚合]]
