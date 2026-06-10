---
type: source
status: active
source_path: raw/repos/2026-06-03-github-openbmb-voxcpm/voxcpm.md
source_type: repo
source_url: https://github.com/OpenBMB/VoxCPM
source_bundle: raw/repos/2026-06-03-github-openbmb-voxcpm
title: GitHub - VoxCPM
authors:
  - OpenBMB
created_at: 2026-06-03
updated_at: 2026-06-03
tags:
  - TTS
  - Voice Cloning
  - Audio
  - Review
related_methods: []
related_concepts: []
related_topics:
  - 语音生成与音频模型
  - 机器学习工程入口
related_cases: []
related_relations: []
---

# GitHub - VoxCPM

## 一句话总结

VoxCPM 是 OpenBMB 的 tokenizer-free TTS 系列，README 当前主推 VoxCPM2，覆盖多语言语音生成、voice design、controllable voice cloning 和 48kHz 输出。

## 当前范围

本页只整理 README 和 GitHub 元数据；不运行语音克隆，不生成仿冒音频，不迁出绕同意采集或伪造身份的操作。

## 摘要

- README 把 VoxCPM 描述为 tokenizer-free Text-to-Speech system，使用 diffusion autoregressive architecture 直接生成连续语音表示。
- VoxCPM2 被描述为 2B 参数、30 语言、超过 200 万小时多语言语音数据训练，支持 Voice Design、Controllable Voice Cloning、Ultimate Cloning 和 48kHz 输出。
- README 提供 Hugging Face、ModelScope、ReadTheDocs、Demo Page 和 playground 入口。
- Quick Start 包含 Python API、CLI、streaming、fine-tuning、production deployment 等入口。

## 证据或原文线索

- GitHub API 抓取时显示 Apache-2.0 license，stars 约 25.2k，仓库未归档。
- GitHub 描述为 “Tokenizer-Free TTS for Multilingual Speech Generation, Creative Voice Design, and True-to-Life Cloning”。
- README News 记录 VoxCPM2 于 2026-04 发布。

## 当前可支持的判断

- 当前来源支持：VoxCPM 是开源语音生成 / TTS / voice cloning 模型样本。
- 当前可保守迁出：它适合支撑 [[语音生成与音频模型]]，也可作为 [[机器学习工程入口]] 中多模态模型工程样本。

## 当前边界

- voice cloning 必须以授权、同意和身份安全为前提。
- 不把 “commercial-ready” 直接写成所有下游场景都无风险；声音权利、肖像权、平台规则和合成内容标注仍需独立判断。
- README 的性能、语种覆盖、克隆质量和部署成本未复测。

## 相关主题

- [[语音生成与音频模型]]
- [[机器学习工程入口]]

## 关系

- `支持` -> [[语音生成与音频模型]]：提供 TTS、voice design 和 voice cloning 模型样本。
- `补充` -> [[机器学习工程入口]]：提供多模态模型从权重、API、CLI 到部署文档的工程入口样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-03-github-openbmb-voxcpm/voxcpm.md](../../raw/repos/2026-06-03-github-openbmb-voxcpm/voxcpm.md)
