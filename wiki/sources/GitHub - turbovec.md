---
type: source
status: active
source_path: raw/repos/2026-06-09-github-ryancodrai-turbovec/turbovec.md
source_type: repo
source_url: https://github.com/RyanCodrai/turbovec
source_bundle: raw/repos/2026-06-09-github-ryancodrai-turbovec
title: GitHub - turbovec
authors:
  - RyanCodrai
created_at: 2026-06-09
updated_at: 2026-06-09
tags:
  - Vector Search
  - Retrieval
  - Rust
  - Review
related_methods: []
related_concepts:
[]
related_topics:
  - Agent 记忆与知识图谱
  - 机器学习工程入口
related_cases: []
related_relations: []
---

# GitHub - turbovec

## 一句话总结

turbovec 是一个基于 TurboQuant 的向量索引，用 Rust 实现并提供 Python bindings，主打压缩、检索速度和可过滤的 hybrid retrieval。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未安装 Python / Rust 包，未跑 recall、compression、speed benchmark，也未接入真实 embedding 或检索服务。

## 摘要

- README 展示 Python 和 Rust 使用方式，并强调 external system 先缩小 candidate ids、再在候选集内 dense rerank 的 hybrid retrieval。
- README 给出 framework integrations、recall、compression、search speed 和 ARM / x86 benchmark 章节。
- 项目语言在 GitHub API 中显示为 Python，README 说明底层由 Rust 与 Python bindings 组成。
- GitHub API 抓取时显示 Python 仓库，MIT license，stars 约 9027，仓库未归档。

## 当前可支持的判断

- 当前来源支持：turbovec 是向量检索 / rerank 基础设施样本。
- 它轻量补充 [[Agent 记忆与知识图谱]]：长期 agent 记忆和 RAG 不只需要存储，还会碰到索引压缩、候选过滤、rerank 和延迟。
- 它也补充 [[机器学习工程入口]] 中“模型能力落地时还要看检索、数据结构和性能边界”这一侧。

## 当前边界

- README benchmark 未在本机复测，不能直接迁出性能排序。
- 实际效果取决于 embedding、过滤条件、数据分布、硬件和 recall / latency 目标。
- 当前不判断它与 FAISS、HNSWLib、Qdrant、Milvus 等方案优劣。

## 相关主题

- [[Agent 记忆与知识图谱]]
- [[机器学习工程入口]]

## 关系

- `补充` -> [[Agent 记忆与知识图谱]]：提供本来源在该主题下的主要样本。
- `轻量补充` -> [[机器学习工程入口]]：提供相邻问题的补充样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-09-github-ryancodrai-turbovec/turbovec.md](../../raw/repos/2026-06-09-github-ryancodrai-turbovec/turbovec.md)
