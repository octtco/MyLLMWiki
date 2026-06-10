---
type: source
status: active
source_path: raw/web/2026-05-21-cslikai-hive/hive.md
source_type: web
source_url: https://cslikai.cn/Hive/
source_bundle: raw/web/2026-05-21-cslikai-hive
title: CSLikAI - Hive 项目页
authors:
  - Kai Li
  - Jintao Cheng
  - Chang Zeng
  - Zijun Yan
  - Helin Wang
  - Zixiong Su
  - Bo Zheng
  - Xiaolin Hu
created_at: 2026-05-21
updated_at: 2026-05-21
tags:
  - Audio
  - Dataset
  - Machine Learning
related_methods: []
related_concepts:
  - 质量指标
related_topics:
  - 音频分离数据集与监督纯度
related_cases:
  - Hive 音频数据集构造案例
related_relations:
  - 数据监督纯度 - 影响 - 模型效果
---

# CSLikAI - Hive 项目页

## 一句话总结

Hive 项目页最稳的价值，是把“监督信号纯度”放到 query-based universal sound separation 的数据效率问题中心。

## 当前范围

本页只整理 Hive 官方项目页，不把 demo 音频样本全部搬入库，也不验证模型权重或完整实验复现。

## 摘要

- 项目页把问题定位为 query-based universal sound separation：从混合声音里按文本查询分离目标声源。
- 它认为现有 in-the-wild 数据常有弱标签和事件共现，容易让模型学到背景噪声与目标类别的伪相关。
- Hive 的路线是先挖出高纯度单事件片段，再按语义一致的方式合成混合音频。
- 项目页给出的管线有三段：ontology reconstruction 与预处理、single-source semantic-acoustic alignment、super-resolution-based standardization。
- 项目页展示了数据组成、混合分布、标签统计、性能和效率图，并提供 2mix 到 5mix 的交互 demo。

## 证据或原文线索

- 页面标题：`A Semantically Consistent Dataset for Data-Efficient Query-Based Universal Sound Separation`
- 项目页链接到 arXiv、GitHub 和 Hugging Face Dataset。
- 页面正文称 Hive 约为 `2k hours of audio`，并强调用约 `0.2%` 的百万小时基线数据规模取得有竞争力的分离表现。

## 当前可支持的判断

- 当前来源支持：在音频分离任务里，弱标签和事件共现本身会构成训练瓶颈。
- 当前可以低强度迁出：当监督信号足够纯时，数据规模不一定是训练效果的唯一主变量。

## 当前边界

- 项目页是项目方自述，不能单独支持“Hive 已全面优于所有大规模音频数据集”。
- 项目页口径是 `2k hours`，与 arXiv 摘要的 `2.4k hours`、GitHub README 的 `2,442 hours` 需要并列保留。
- demo 样本可用于直观看效果，但不等于独立 benchmark。

## 相关概念

- [[质量指标]]

## 相关主题

- [[音频分离数据集与监督纯度]]

## 关系

- `支持` -> [[音频分离数据集与监督纯度]]：提供项目页层面的管线、图示和 demo 证据。

## 回链

- 对应来源包主文件：[raw/web/2026-05-21-cslikai-hive/hive.md](../../raw/web/2026-05-21-cslikai-hive/hive.md)
