---
type: source
status: review
source_path: raw/repos/2026-06-08-github-ggml-org-whisper-cpp/whisper-cpp.md
source_type: repo
source_url: https://github.com/ggml-org/whisper.cpp
source_bundle: raw/repos/2026-06-08-github-ggml-org-whisper-cpp
title: GitHub - whisper.cpp
authors:
  - ggml-org
created_at: 2026-06-08
updated_at: 2026-06-08
tags:
  - Audio
  - ASR
  - Inference
  - Review
related_methods: []
related_concepts: []
related_topics:
  - 语音生成与音频模型
  - 机器学习工程入口
related_cases: []
related_relations: []
---

# GitHub - whisper.cpp

## 一句话总结

whisper.cpp 是 OpenAI Whisper 自动语音识别模型的高性能 C/C++ 推理实现，强调轻量、跨平台、量化、CPU/GPU 支持和移动端 / WebAssembly / 嵌入式集成。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未下载模型、未编译、未转写音频，也未复测各硬件后端性能。

## 摘要

- README 把 whisper.cpp 定位为 OpenAI Whisper ASR model 的 high-performance inference 实现。
- 特性包括无依赖 C/C++、Apple Silicon / Metal / Core ML、AVX、Vulkan、NVIDIA GPU、AMD ROCm、OpenVINO、Ascend NPU、量化和 C-style API。
- 支持平台覆盖 macOS、iOS、Android、Java、Linux、FreeBSD、WebAssembly、Windows、Raspberry Pi 和 Docker。
- GitHub API 抓取时显示 C++ 仓库，MIT license，stars 约 50545，仓库未归档。

## 当前可支持的判断

- 当前来源支持：whisper.cpp 是语音识别 / 音频模型本地推理工程化样本。
- 当前可保守迁出：它补充 [[语音生成与音频模型]]，让该页从 TTS / voice cloning 扩到 ASR 与本地推理。
- 它也能轻量补充 [[机器学习工程入口]] 中“模型工程化、量化、跨平台推理”的样本。

## 当前边界

- README 的后端支持和性能需要按具体硬件、模型大小、量化格式和音频格式复测。
- 语音转写涉及隐私、录音授权和敏感内容处理，后续应用要先定数据边界。
- 当前不把 quick start 片段升级成完整部署教程。

## 相关主题

- [[语音生成与音频模型]]
- [[机器学习工程入口]]

## 回链

- 对应来源包主文件：[raw/repos/2026-06-08-github-ggml-org-whisper-cpp/whisper-cpp.md](../../raw/repos/2026-06-08-github-ggml-org-whisper-cpp/whisper-cpp.md)
