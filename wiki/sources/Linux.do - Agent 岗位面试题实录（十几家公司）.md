---
type: source
status: review
source_path: raw/web/2026-06-10-linuxdo-topic-2365650-agent-job-interview-questions/agent-job-interview-questions.md
source_type: web
source_url: https://linux.do/t/topic/2365650
source_bundle: raw/web/2026-06-10-linuxdo-topic-2365650-agent-job-interview-questions
title: Linux.do - Agent 岗位面试题实录（十几家公司）
authors:
  - guava_16
created_at: 2026-06-10
updated_at: 2026-06-10
temporal_status: current
confidence: medium
claim_status: review
tags:
  - Agent
  - 面试
  - RAG
  - 求职
  - 前端转型
related_methods: []
related_concepts: []
related_topics:
  - Agent 框架设计
  - Agent 记忆与知识图谱
related_cases: []
related_relations: []
---

# Linux.do - Agent 岗位面试题实录（十几家公司）

## 一句话总结

一位前端被裁后转投 Agent 岗位的求职者，把十几家公司的面试录音用 AI 整理成按公司分组的面试题清单，当前最有价值的不是题目本身，而是它作为"2026 年中 Agent 岗位市场实际在考什么"的需求侧快照。

## 当前范围

本页只整理这份题单作为市场信号样本的来源意义，不逐题给参考答案，也不把题目清单升成学习大纲。题目由录音经 AI 整理，措辞可能与面试官原话有出入。

## 摘要

- 作者背景：前端开发，上月被裁，学了一些 AI 课程后面试了十几家 Agent 岗位（穿插前端 / 全栈岗），全程录音并用 AI 整理出题目，按 11 家公司（化名缩写）分组。
- Agent / AI 题高频集中在几个簇：多 Agent 架构（为什么需要、什么场景、和单 Agent 多职能的区别）、RAG 全链路（流程、检索加速、向量库选型、召回准确性、混合检索后为什么还要精排）、上下文治理（压缩策略、压缩质量兜底）、意图识别与动态路由、查询改写。
- 出现了对 Claude Code 的针对性考察：多层架构、上下文治理、核心循环流程、泄露事件源码研究——agent 产品的内部机制已经成为面试考点。
- 成本和规模问题占比明显：token 消耗量、成本优化方案及降本幅度、AI 投入前后收益、用户量 / 日活 / 并发——岗位预期不只是会搭，还要会算账。
- 工程基建题持续在场：SSE 断线续传、WebSocket 心跳重连降级、消息队列任务不丢失、断点续跑、重复推理去重、k8s 多租户部署。
- AI 工作流题成为通用题型：个人 AI 开发工作流、用什么 MCP / Skill、AI 编程规范、AI 代码的 code review、无设计稿时用 AI 出原型。
- 也有相当比例的传统前端 / 后端八股（Vue 响应式、ES6、秒杀系统、MySQL 优化），说明这批"Agent 岗"实际上多是全栈底子加 AI 能力的复合岗。
- 评论区切片显示同类转型需求真实存在（找实习、问转型路线、问技术栈建议）。

## 证据或原文线索

- 原帖链接：`https://linux.do/t/topic/2365650`
- 正文按 ML / KJ / JR / TK / YC / HJ / FN / XZ / SH / PY / HQ / YU 等公司分组，共约 200 道题。
- JR 公司题组：`怎么加速 RAG 的检索过程`、`上下文压缩的策略`、`claude code 的核心循环流程`。
- HQ 公司题组：`混合检索已经做过分组、排序、去重，为什么还需要再次精排（Re-rank）`、`任务重试会造成重复执行、重复调用大模型，如何做重复推理优化`、`解释下 Harness 相关概念`。
- ML 公司题组：`单个 Agent 其实也可以分配多个职能，为什么还要多 Agent`、`做了哪些成本优化方案？最终降了多少成本`。
- 作者自述：`面试过程都录音了，然后让 AI 整理了一下面试官提问的问题`。

## 当前可支持的判断

- 当前来源支持：2026 年中国内 Agent 岗位面试的考察重心是"多 Agent 架构判断 + RAG 全链路 + 上下文治理 + 成本核算"，而不只是会调 LangChain API。
- 当前来源支持：Claude Code 这类 agent 产品的内部机制（架构、上下文治理、核心循环）已进入面试考点，agent harness 知识有了求职市场上的直接变现场景。
- 当前可保守迁出：这批"Agent 岗"多数仍要求扎实的全栈工程底子（消息队列、SSE/WS、数据库优化），AI 能力是叠加项而非替代项。
- 更强结论仍待验证：单一作者、单一时间窗、岗位偏前端/全栈背景，不能直接外推为"Agent 岗位市场全貌"；题目经 AI 转写，个别表述可能失真。

## 当前边界

- 公司均为化名缩写，无法核对岗位 JD 和城市 / 薪资区间。
- 题目按录音转写整理，可能存在转写误差和遗漏追问语境。
- 不逐题写参考答案，不把题单升成"Agent 面试准备方法页"。
- 评论区只保留 2-6 楼切片，后续讨论未跟踪。

## 相关概念

- 待补

## 相关方法

- 待补

## 相关主题

- [[Agent 框架设计]]
- [[Agent 记忆与知识图谱]]

## 相关案例

- 待补

## 关系

- `补充` -> [[Agent 框架设计]]：从求职市场需求侧反推 Agent 工程能力清单（多 Agent 取舍、上下文治理、成本核算），与该主题里框架供给侧样本互补。
- `补充` -> [[Agent 记忆与知识图谱]]：印证 RAG 全链路（检索加速、混合检索、精排、查询改写）已是岗位标配考点。
- `补充` -> [[Linux.do - RAG 全流程实现教程（Java + 完整代码）]]：JR / HQ 公司的 RAG 题组（流程、查询改写、为什么要精排）与该教程覆盖的工程环节几乎一一对应，一供一需。
- `补充` -> [[Linux.do - AI 产品经理简历与面试建议]]：同属 AI 转型求职线索，一个偏研发岗实录，一个偏产品岗建议。

## 回链

- 对应原始文件：[raw/web/2026-06-10-linuxdo-topic-2365650-agent-job-interview-questions/agent-job-interview-questions.md](../../raw/web/2026-06-10-linuxdo-topic-2365650-agent-job-interview-questions/agent-job-interview-questions.md)
