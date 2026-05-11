---
type: source
status: active
source_path: raw/web/2026-04-23-zhihu-2024232028762112639-karpathy-llm-wiki/karpathy-llm-wiki.md
source_type: web
source_url: https://zhuanlan.zhihu.com/p/2024232028762112639
source_bundle: raw/web/2026-04-23-zhihu-2024232028762112639-karpathy-llm-wiki
title: 知乎专栏 - Karpathy 的 LLM Wiki 新范式
authors:
  - 新智元​人工智能话题下的优秀答主
created_at: 2026-04-27
updated_at: 2026-04-27
tags:
  - 知识管理
  - LLM Wiki
  - 个人知识库
related_concepts: []
related_topics: []
related_relations: []
---

# 知乎专栏 - Karpathy 的 LLM Wiki 新范式

## 一句话总结

这篇中文转述文章把 Karpathy 的 LLM Wiki 思路讲得很集中：它真正补强的不是某个工具，而是“raw / wiki / schema / ingest / query / file-back / lint”这一套个人知识库运行框架。

## 摘要

- 文章把 LLM Wiki 的核心对比压在“RAG 每次重新发现，wiki 会持续积累”上，强调不是只做检索，而是把原始资料编译成一套可导航知识结构。
- 正文把整套骨架拆成三层：原始资料层、Wiki 层、规则文件层，并把日常操作收成 ingest、query、file back、lint 四步。
- Farzapedia 这一段进一步说明，这套东西不只想管理公开资料，也想把个人日记、笔记、聊天和审美线索编译成给 agent 用的百科。

## 证据或原文线索

- 文中明确把 raw/、wiki 和 schema 说成整套系统骨架，并反复强调“Obsidian 是 IDE，大模型是程序员，Wiki 是代码库”。
- “导入、查询、回填、自检”被写成四个核心操作，而且特别强调查询结果也要继续存回 wiki。
- Farzapedia 的例子把“把个人资料编译成 agent 可爬取百科”讲得很具体，这和当前仓库正在补的对象层、行动层方向直接相关。

## 我的判断

- 这份来源足够作为当前个人 LLM Wiki 升级工作的方向性补强材料。
- 它最适合当前仓库的方式，不是立刻再抽新主题页，而是先接回已有的两份升级方案与路由细则。
- 但它仍然主要是中文二手传播材料；如果后面要把 Karpathy 的具体设计口径说得更准，最好继续补一手原帖或实作材料。

## 相关输出

- [[2026-04-24-个人-LLM-Wiki-结构升级方案-v0.2]]
- [[2026-04-24-个人-LLM-Wiki-模板与路由细则-v0.3]]

## 相关概念

- 暂无

## 相关主题

- 暂无

## 关系

- `二手传播` -> Karpathy 的 LLM Wiki 设想：这篇来源主要承担中文转述和放大作用，而不是一手原帖。
- `补充` -> 当前仓库升级方向：它直接补强了 raw / wiki / schema / ingest / lint 这一套知识库运行想象。

## 回链

- 对应来源包主文件：[raw/web/2026-04-23-zhihu-2024232028762112639-karpathy-llm-wiki/karpathy-llm-wiki.md](../../raw/web/2026-04-23-zhihu-2024232028762112639-karpathy-llm-wiki/karpathy-llm-wiki.md)
