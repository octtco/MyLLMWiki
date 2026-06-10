---
type: source
status: active
source_path: raw/repos/2026-06-09-github-andyyyy64-whichllm/whichllm.md
source_type: repo
source_url: https://github.com/Andyyyy64/whichllm
source_bundle: raw/repos/2026-06-09-github-andyyyy64-whichllm
title: GitHub - whichllm
authors:
  - Andyyyy64
created_at: 2026-06-09
updated_at: 2026-06-09
tags:
  - Local LLM
  - Benchmark
  - Hardware
  - Review
related_methods: []
related_concepts:
[]
related_topics:
  - AI 工具化知识工作流
  - 机器学习工程入口
related_cases: []
related_relations: []
---

# GitHub - whichllm

## 一句话总结

whichllm 是一个根据本机硬件和真实 benchmark 推荐可运行本地 LLM 的命令行工具，强调按近期性能而不是参数量选模型。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未安装 CLI，未测试 GPU/CPU 检测、GGUF 选择、chat、JSON 输出或硬件升级比较。

## 摘要

- GitHub 描述强调 “Find the local LLM that actually runs and performs best on your hardware”。
- README 提供 best models for this machine、pretend GPU、compare upgrade candidates、find GPU needed for a model、start chat、print Python、return JSON 等工作流。
- README 明确强调 recency-aware benchmarks 和本机硬件适配。
- GitHub API 抓取时显示 Python 仓库，MIT license，stars 约 3537，仓库未归档。

## 当前可支持的判断

- 当前来源支持：whichllm 是本地模型选择和硬件适配工具样本。
- 它补充 [[机器学习工程入口]]：模型选择不是只看参数量，还要看硬件、量化格式、速度、内存和实际任务。
- 它也补充 [[AI 工具化知识工作流]]：本地 LLM 选型可以变成脚本化、可集成的决策步骤。

## 当前边界

- benchmark 来源、更新时间和硬件映射未复核。
- 不同任务的质量、上下文长度、工具调用能力和许可不能只由“能跑/跑得快”决定。
- 当前不把它当本地 LLM 采购建议，只保存为选型工具样本。

## 相关主题

- [[AI 工具化知识工作流]]
- [[机器学习工程入口]]

## 关系

- `补充` -> [[AI 工具化知识工作流]]：提供本来源在该主题下的主要样本。
- `轻量补充` -> [[机器学习工程入口]]：提供相邻问题的补充样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-09-github-andyyyy64-whichllm/whichllm.md](../../raw/repos/2026-06-09-github-andyyyy64-whichllm/whichllm.md)
