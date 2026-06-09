---
type: topic
status: review
tags:
  - Agent Memory
  - Knowledge Graph
  - Retrieval
related_topics:
  - Agent 框架设计
  - AI 工具化知识工作流
  - 代码库图谱化理解
related_methods: []
related_concepts:
  - 可观测性
related_relations: []
source_pages:
  - GitHub - Personal AI Infrastructure
  - GitHub - turbovec
  - GitHub - Graphiti
  - GitHub - Supermemory
  - GitHub - Production Agentic RAG Course
  - GitHub - Noema
updated: 2026-06-09
---

# Agent 记忆与知识图谱

## 这页真正想回答什么

这页想回答的是：agent 的长期记忆什么时候不该只是一段聊天历史或一组文档 chunk，而需要更结构化的图谱层。

## 为什么这个问题容易散

谈 agent 记忆时，很容易只问“存了多少上下文”。但长期运行的 agent 真正麻烦的地方不是存储量，而是事实会变、来源会混、关系会交叉、用户会在不同时间给出互相覆盖的信息。只存文本，常常很难回答“现在什么为真”“以前什么为真”“这个判断来自哪段原始材料”。

## 当前最稳的主线

[[GitHub - Graphiti]] 当前给出的入口，是把 agent memory 写成 temporal context graph。它把实体、关系、事实、时间有效窗口和 episodes provenance 放在同一个结构里，让记忆不只是“召回相关文本”，而是能围绕事实变化和来源回溯组织上下文。

这条线和 [[Agent 框架设计]] 的关系很直接：如果 agent 框架要长期运行，只靠 skill / SOP 沉淀经验还不够，它还需要知道工作对象、用户偏好、企业数据和外部事实怎样随时间变化。它也和 [[可观测性]] 相邻，因为图谱层的意义之一，就是让系统知道自己到底看见了哪些状态线索，以及这些线索从哪里来。

[[GitHub - Supermemory]] 把同一问题推向产品和 API 形态：它不只讲图谱结构，还把 memory、user profiles、hybrid search、connectors、file processing 和 MCP server 包成一个上下文服务。这样这页可以保守地区分两条路线：Graphiti 更像可自管的 temporal context graph engine，Supermemory 更像完整 memory / context stack。

[[GitHub - Production Agentic RAG Course]] 则补了更教学化的工程路径：先用 OpenSearch / BM25 打底，再做 chunking、hybrid search、RAG、Langfuse tracing、Redis caching，最后加入 LangGraph 的 document grading、query rewriting 和 out-of-domain guardrails。它不直接等于 agent memory 产品，但能补这页里 retrieval layer 和 agentic RAG 的生产化练习样本。

[[GitHub - Noema]] 提供的是更轻的一层本地持久记忆样本：README 里提到 SQLite 保存 conversation turns、summaries、user profile 和 task runs。它还不到 Graphiti 那种 temporal context graph，也不是 Supermemory 那种 memory / context API，但能说明桌面 companion 需要把对话记忆、用户画像和任务运行记录接进交互体验里。

[[GitHub - turbovec]] 从索引层补了一块：agent memory 和 RAG 要长期可用，不只需要“记住”，还要处理向量压缩、候选过滤、dense rerank、召回率和延迟。[[GitHub - Personal AI Infrastructure]] 则从个人基建侧补充 memory that compounds 和 filesystem context 这类理念，但当前还不能等同于已验证的图谱记忆系统。

## 当前边界

- 当前只有 Graphiti、Supermemory、Production Agentic RAG Course 和 Noema 四个来源支撑，先不把“知识图谱”“GraphRAG”“context graph”拆成独立概念页。
- README 对 GraphRAG 的比较和低延迟口径未复测。
- Supermemory 的 benchmark 排名、隐私边界和连接器权限没有实测。
- Production Agentic RAG Course 的 Docker、OpenSearch、Langfuse、Redis 和 Telegram Bot 链路未实测。
- Noema 的 SQLite 记忆、用户画像和 task runs 只按 README 保存，未验证隐私、清理、导出或权限边界。
- 这页暂时只组织 agent memory 方向，不讨论通用知识图谱工程。

- turbovec 的 recall、compression 和 speed benchmark 未复测；Personal AI Infrastructure 的 memory / filesystem context 当前仍是 README 理念与项目入口，未验证实现边界。

## 代表性来源

- [[GitHub - Personal AI Infrastructure]]
- [[GitHub - turbovec]]
- [[GitHub - Graphiti]]
- [[GitHub - Supermemory]]
- [[GitHub - Production Agentic RAG Course]]
- [[GitHub - Noema]]

## 相关概念

- [[可观测性]]

## 相关主题

- [[Agent 框架设计]]
- [[AI 工具化知识工作流]]
- [[代码库图谱化理解]]
