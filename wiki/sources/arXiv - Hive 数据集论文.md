---
type: source
status: review
source_path: raw/papers/2026-01-30-arxiv-2601-22599-hive/README.md
source_type: paper
source_url: https://arxiv.org/abs/2601.22599
source_bundle: raw/papers/2026-01-30-arxiv-2601-22599-hive
title: arXiv - Hive 数据集论文
authors:
  - Kai Li
  - Jintao Cheng
  - Chang Zeng
  - Zijun Yan
  - Helin Wang
  - Zixiong Su
  - Bo Zheng
  - Xiaolin Hu
year: 2026
created_at: 2026-05-21
updated_at: 2026-05-21
tags:
  - Audio
  - Dataset
  - Paper
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

# arXiv - Hive 数据集论文

## 一句话总结

这篇论文入口最值得记住的是：Hive 把音频分离的数据效率问题重写成“监督纯度优先”的数据构造问题。

## 当前范围

本页整理 arXiv 摘要页和已入库 PDF，不做全文逐节拆解；如果后续要深入实验表格和消融，再另建 `outputs/` 工作层。

## 摘要

- 论文研究 query-based universal sound separation，即按查询从混合音频中分离目标声源。
- 摘要把现有方法的残余干扰问题追到数据瓶颈：in-the-wild 数据有弱标签和严重事件共现。
- 论文提出用语义一致的合成协议，从野外数据中挖高纯度单事件片段，再构造 Hive。
- arXiv 摘要称 Hive 包含 `2.4k hours of raw audio`。
- 摘要说部分开源模型在 Hive 上训练后，可与使用约 500 倍更大训练数据的 SAM-Audio 形成竞争，并在 OOD benchmark 上表现出 zero-shot generalization。

## 证据或原文线索

- arXiv ID：`2601.22599`
- 提交日期：2026-01-30
- 学科：`Sound (cs.SD); Human-Computer Interaction (cs.HC)`
- 评论：`Technical Report`
- DOI：`https://doi.org/10.48550/arXiv.2601.22599`

## 当前可支持的判断

- 当前来源支持：对音频分离模型来说，事件共现和弱标签会诱发伪相关，而更纯的监督信号可能显著改善数据效率。
- 当前可以低强度迁出：在某些机器学习任务中，数据质量与构造协议可能比单纯扩大数据规模更值得优先检查。

## 当前边界

- 本页目前只整理摘要层判断；全文实验细节尚未拆解。
- `500 倍更大数据`、OOD generalization 等说法先按论文摘要口径保留，不扩成普遍结论。
- 与项目页和 README 的规模口径差异需要保留，不强行改写成一个单一数字。

## 相关概念

- [[质量指标]]

## 相关主题

- [[音频分离数据集与监督纯度]]

## 关系

- `支持` -> [[音频分离数据集与监督纯度]]：提供论文层面的研究问题、数据瓶颈和实验结论口径。
- `补充` -> [[GitHub - Hive]]：论文摘要提供研究主张，仓库 README 提供发布和脚本入口。

## 回链

- 对应来源包入口：[raw/papers/2026-01-30-arxiv-2601-22599-hive/README.md](../../raw/papers/2026-01-30-arxiv-2601-22599-hive/README.md)
- PDF：[raw/papers/2026-01-30-arxiv-2601-22599-hive/files/2601.22599v1.pdf](../../raw/papers/2026-01-30-arxiv-2601-22599-hive/files/2601.22599v1.pdf)
