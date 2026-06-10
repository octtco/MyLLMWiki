---
type: source
status: active
source_path: raw/repos/2026-05-21-github-jusperlee-hive/hive.md
source_type: repo
source_url: https://github.com/JusperLee/Hive
source_bundle: raw/repos/2026-05-21-github-jusperlee-hive
title: GitHub - Hive
authors:
  - JusperLee
created_at: 2026-05-21
updated_at: 2026-05-21
tags:
  - Audio
  - Dataset
  - Repository
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

# GitHub - Hive

## 一句话总结

Hive 仓库 README 最稳的价值，是把项目页里的想法具体落到数据发布形态、生成管线和可用脚本上。

## 当前范围

本页只整理仓库 README 快照，不 clone 完整代码树，不验证 Hugging Face 权重，也不跑推理脚本。

## 摘要

- README 把 Hive 定义为用于 Universal Sound Separation 的高质量合成数据集。
- 它给出更细的规模口径：`2,442 hours of raw audio`、`19.6M mixtures`、`283 sound categories`、`44.1kHz`。
- 数据发布分成两种：metadata-only 的 `JusperLee/Hive`，以及预生成混合音频的 `JusperLee/Hive-ALL`。
- 管线被拆成 6 步：切分音频、单标签过滤、Qwen3-Omni 单事件过滤、AudioTag 标注、Qwen3-Omni 叶节点分类、Apollo 超分。
- 仓库提供 `infer_audiosep.py`、`infer_flowsep.py` 和 Gradio demo，用于 AudioSep-hive 与 FlowSep-hive 的推理体验。

## 证据或原文线索

- README 标注 Apache 2.0 项目许可证。
- 2026-05-19 README news 说 Hive-ALL 以 285 GB WebDataset 格式发布。
- 2026-05-21 README news 说 Hive-ALL 也提供 ModelScope 镜像。
- README 明确不重新分发原始数据集音频，只发布元数据或生成后的混合音频形态。

## 当前可支持的判断

- 当前来源支持：Hive 不只是论文概念，还提供了可操作的数据构造、发布和推理入口。
- 当前可以低强度迁出：音频数据集工程里的“可复现”可以通过 metadata-only 与 pre-generated audio 两种发布形态分别处理。

## 当前边界

- README 不能替代论文实验细节，也不能证明第三方实际训练效果。
- Hive-ALL 体积较大，知识库只记录入口，不下载数据集。
- README 的数据规模口径与项目页、arXiv 摘要存在轻微表述差异，应保留来源差异。

## 相关概念

- [[质量指标]]

## 相关主题

- [[音频分离数据集与监督纯度]]

## 关系

- `补充` -> [[CSLikAI - Hive 项目页]]：仓库 README 补足项目页之外的数据发布和脚本入口。
- `支持` -> [[音频分离数据集与监督纯度]]：提供数据规模、管线步骤和发布方式证据。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-21-github-jusperlee-hive/hive.md](../../raw/repos/2026-05-21-github-jusperlee-hive/hive.md)
