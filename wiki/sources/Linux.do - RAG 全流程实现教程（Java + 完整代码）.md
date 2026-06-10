---
type: source
status: review
source_path: raw/web/2026-06-10-linuxdo-topic-2364008-rag-java-fullstack-tutorial/rag-java-fullstack-tutorial.md
source_type: web
source_url: https://linux.do/t/topic/2364008
source_bundle: raw/web/2026-06-10-linuxdo-topic-2364008-rag-java-fullstack-tutorial
title: Linux.do - RAG 全流程实现教程（Java + 完整代码）
authors:
  - worenbudaoni
created_at: 2026-06-10
updated_at: 2026-06-10
temporal_status: current
confidence: medium
claim_status: review
tags:
  - RAG
  - Java
  - LangChain4j
  - Embedding
  - Reranker
  - 向量数据库
related_methods: []
related_concepts: []
related_topics:
  - Agent 记忆与知识图谱
related_cases: []
related_relations: []
---

# Linux.do - RAG 全流程实现教程（Java + 完整代码）

## 一句话总结

这篇帖子用 Java + LangChain4j 0.35 把 RAG 的入库和提问两条流程完整走了一遍，并给出配套开源仓库 `worenbudaoni/rag-study-helper`，当前最适合作为 RAG 工程化全流程的教学样本。

## 当前范围

本页只整理帖子正文和评论区切片的来源意义，未对配套 GitHub 仓库做 repo 快照，也未实际运行代码验证教程口径。

## 摘要

- 作者按 Linux.do 开源推广规则发帖，宣称项目完整开源，配套仓库为 `worenbudaoni/rag-study-helper`（jdk8 + langchain4j 0.35）。
- 帖子把 RAG 拆成两条流程：入库流程 `文件 -> 分割器 -> Embedding -> 向量数据库`，提问流程 `问题 -> 问题重写 -> Embedding -> 向量检索 -> 相关性筛选 -> rerank -> prompt 优化 -> LLM 回答`。
- 问题重写给出了一个具体的触发启发式：提问小于 5 个字且包含“他、她、它、上述”等指代词时才重写，避免每次都重写浪费时间和 token。
- 相关性筛选用余弦相似度阈值（作者设 0.77）过滤检索结果，并强调阈值跟模型、文档、问题都有关，需要打日志观测调试。
- rerank 的定位是“检索召回 top 20，但真正有价值的可能只有 3-5 条”，通过重排提升上下文质量、省 token；作者用硅基流动 API 手搓了 `bge-reranker-v2-m3` 的调用。
- 工程细节包括：文件 hash 判重、按 token 分割（512 上限减去文件名前缀）、embedding 批量请求（10 条一批、失败降级逐条）、向量 ID 与关系型数据库分片记录对应。
- 帖子末尾给出向量数据库（9 款）、Embedding 模型（8 款）、Reranker（9 款）、分割器（7 款）四张选型对照表，并强调嵌入模型切换后向量数据全部作废。
- 评论区切片保留了作者对流程图歧义的更正：增强 prompt（重写后的问题）只用于检索，最终喂给 LLM 的仍是用户原始问题。

## 证据或原文线索

- 原帖链接：`https://linux.do/t/topic/2364008`
- 配套仓库：`https://github.com/worenbudaoni/rag-study-helper`
- 原文代码段：`LangChain4jConfig.java`（InMemory / Chroma / Milvus 三套向量库配置）、`DocumentIngestionService.java`（判重、解析、分割、批量嵌入）、`RagQueryService.java`（提问主流程）、`RerankService.java`（硅基流动 rerank API 调用）。
- 原文写明作者所用组合：`BAAI/bge-large-zh-v1.5`（1024 维 / 512 token 上限）+ `BAAI/bge-reranker-v2-m3` + DeepSeek 官方 LLM。
- 评论区 22 楼截图（`images/006.png`）与作者回复，明确“询问 LLM 的问题无论如何都是用户的原始问题（非增强）”。

## 当前可支持的判断

- 当前来源支持：RAG 的最小工程闭环可以拆成入库、提问两条流水线，每个环节（分割、嵌入、筛选、重排、prompt 约束）各自有明确的失败模式和调参点。
- 当前来源支持：问题重写、相似度阈值、rerank topN 这类参数没有标准值，作者的做法是条件触发 + 日志观测，而不是套用固定配置。
- 当前可保守迁出：嵌入模型一旦切换，存量向量数据全部作废，这是 RAG 系统选型时需要前置锁定的约束。
- 当前可保守迁出：检索用的查询（重写/增强后）和喂给 LLM 的问题（用户原始问题）应当分离，这是评论区确认过的设计点。
- 更强结论仍待验证：教程代码是否能按 README 跑通、选型对照表中的参数口径（维度、上下文上限、榜单名次）是否准确，本轮未复核。

## 当前边界

- 配套仓库 `rag-study-helper` 本轮未做 repo 快照，代码结构、依赖和可运行性未验证。
- 四张选型对照表是作者单方整理，部分条目（如榜单排名、推测的上下文上限）带有明显的转述性质，不能直接当事实引用。
- 帖子提到的后续两篇（接入飞书 WIKI 文档、令牌桶限流）尚未发布，本来源只覆盖第一篇。
- 不把教程中的具体参数（0.77 阈值、top 20、batch 10）写成通用最佳实践。

## 相关概念

- 待补（如后续 RAG 来源继续积累，可评估 `问题重写`、`重排序` 是否值得拆概念页）

## 相关方法

- 待补

## 相关主题

- [[Agent 记忆与知识图谱]]

## 相关案例

- 待补

## 关系

- `补充` -> [[Agent 记忆与知识图谱]]：为该主题里的 retrieval layer / agentic RAG 线补一个 Java 技术栈的全流程教学样本。
- `互证` -> [[GitHub - Production Agentic RAG Course]]：两者都覆盖 chunking、hybrid 检索、rerank 和生产化关注点，但本帖是 Java + LangChain4j 路线，对方是 Python + OpenSearch / LangGraph 路线。

## 回链

- 对应原始文件：[raw/web/2026-06-10-linuxdo-topic-2364008-rag-java-fullstack-tutorial/rag-java-fullstack-tutorial.md](../../raw/web/2026-06-10-linuxdo-topic-2364008-rag-java-fullstack-tutorial/rag-java-fullstack-tutorial.md)
