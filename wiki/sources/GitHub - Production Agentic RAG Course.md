---
type: source
status: review
source_path: raw/repos/2026-06-03-github-jamwithai-production-agentic-rag-course/production-agentic-rag-course.md
source_type: repo
source_url: https://github.com/jamwithai/production-agentic-rag-course
source_bundle: raw/repos/2026-06-03-github-jamwithai-production-agentic-rag-course
title: GitHub - Production Agentic RAG Course
authors:
  - jamwithai
created_at: 2026-06-03
updated_at: 2026-06-03
tags:
  - RAG
  - Agent
  - Retrieval
  - Review
related_methods: []
related_concepts:
  - 可观测性
related_topics:
  - Agent 记忆与知识图谱
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - Production Agentic RAG Course

## 一句话总结

Production Agentic RAG Course 是一个以 arXiv Paper Curator 为项目载体的生产级 RAG 学习仓库，从基础设施、数据管线、BM25、hybrid search、RAG、监控缓存推进到 LangGraph agentic RAG 和 Telegram bot。

## 当前范围

本页只整理 README 与 GitHub 元数据；未运行课程项目、Docker Compose、OpenSearch、Airflow、Langfuse 或 Telegram Bot。

## 摘要

- README 把课程定位为 learner-focused project，目标是构建能抓取论文、理解内容并回答研究问题的 research assistant。
- 课程路径从 Week 1 到 Week 7：基础设施、arXiv 数据摄取、OpenSearch/BM25、chunking + hybrid search、完整 RAG、Langfuse/Redis 监控缓存、LangGraph agentic RAG + Telegram Bot。
- README 强调先掌握 keyword search foundations，再增强 vector / hybrid retrieval。
- 技术栈包括 FastAPI、PostgreSQL、OpenSearch、Airflow、Ollama、Langfuse、Redis、LangGraph、Gradio 和 Telegram Bot。

## 证据或原文线索

- GitHub API 抓取时显示 MIT license，stars 约 6.4k，仓库未归档。
- README 标题为 “The Mother of AI Project / Phase 1 RAG Systems: arXiv Paper Curator”。

## 当前可支持的判断

- 当前来源支持：该仓库是生产级 RAG / agentic RAG 学习项目样本。
- 当前可保守迁出：它补充了 [[Agent 记忆与知识图谱]] 中 retrieval 和 agentic RAG 的工程侧，也补充 [[AI 工具化知识工作流]] 中材料进入、检索、监控和交付界面的链路。

## 当前边界

- 未验证课程代码可运行性、服务资源消耗、OpenSearch 配置、Langfuse tracing 或 Telegram Bot 部署。
- 课程口径不能直接等同于生产最佳实践；仍需真实项目跑测。
- arXiv 抓取、论文处理和外部 API key 使用需要遵守对应服务条款。

## 相关主题

- [[Agent 记忆与知识图谱]]
- [[AI 工具化知识工作流]]

## 关系

- `补充` -> [[Agent 记忆与知识图谱]]：提供 RAG、hybrid retrieval、document grading 和 query rewriting 的工程课程样本。
- `补充` -> [[AI 工具化知识工作流]]：提供从 ingest 到检索、监控、缓存和交互界面的生产化链路样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-03-github-jamwithai-production-agentic-rag-course/production-agentic-rag-course.md](../../raw/repos/2026-06-03-github-jamwithai-production-agentic-rag-course/production-agentic-rag-course.md)
