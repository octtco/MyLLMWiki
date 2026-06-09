---
type: entity
entity_type: dataset
status: review
aliases:
  - Hive Dataset
  - JusperLee/Hive
tags:
  - Audio
  - Dataset
  - Machine Learning
related_sources:
  - CSLikAI - Hive 项目页
  - GitHub - Hive
  - arXiv - Hive 数据集论文
related_entities: []
related_goals: []
related_topics:
  - 音频分离数据集与监督纯度
related_methods: []
related_concepts:
  - 质量指标
related_cases:
  - Hive 音频数据集构造案例
updated: 2026-05-21
---

# Hive

## 这是什么

Hive 是一个面向 query-based universal sound separation 的合成音频数据集和数据构造管线。它围绕“先获得高纯度单事件片段，再合成语义一致的混合音频”来降低弱标签和事件共现带来的训练噪声。

## 为什么它现在重要

它不是单纯新增一个音频数据集，而是把模型训练效果的问题往前推到监督信号质量。对当前知识库来说，Hive 是一个可以连接 [[机器学习工程入口]] 和 [[音频分离数据集与监督纯度]] 的样本：先看数据与标签怎样生成，再看模型分数。

## 当前状态

- 项目页、GitHub README、arXiv 论文入口已入库。
- GitHub README 记录 Hive 有 `2,442 hours of raw audio`、`19.6M mixtures`、`283 sound categories`。
- README 提供 metadata-only 的 `JusperLee/Hive` 和预生成混合音频 `JusperLee/Hive-ALL` 两种发布形态。
- 项目页包含交互 demo，仓库提供 AudioSep-hive、FlowSep-hive 推理脚本和 Gradio demo。

## 关键关系

- 与 [[音频分离数据集与监督纯度]]：Hive 是当前该主题的主样本。
- 与 [[质量指标]]：Hive 的主张需要通过分离准确性、感知质量和 OOD benchmark 来判断。
- 与 [[机器学习工程入口]]：Hive 提供了“模型之前先看数据构造”的音频任务版本。

## 最近变化

- 2026-01-30：arXiv 论文提交。
- 2026-05-19：README 记录 Hive-ALL 预生成混合音频发布。
- 2026-05-21：README 记录 Hive-ALL 提供 ModelScope 镜像；本知识库完成首次整理。

## 当前未决问题

- PDF 全文实验表格、消融和具体 benchmark 仍未逐节拆解。
- Hugging Face 数据集卡未成功抓取，后续可再补。
- 项目页 `2k hours`、arXiv `2.4k hours`、README `2,442 hours` 三种口径需作为来源差异保留。

## 相关来源

- [[CSLikAI - Hive 项目页]]
- [[GitHub - Hive]]
- [[arXiv - Hive 数据集论文]]

## 相关知识页

- [[音频分离数据集与监督纯度]]
- [[机器学习工程入口]]
- [[质量指标]]
- [[Hive 音频数据集构造案例]]

## 关系

- `体现` -> [[机器学习工程入口]]：把“先看数据和标签”落到音频分离数据集构造。
- `支持` -> [[音频分离数据集与监督纯度]]：作为当前最完整的来源簇。
