---
type: concept
status: active
aliases:
  - Self-Evolving Agent
tags:
  - Agent
  - GenericAgent
  - Skill
  - Memory
related_concepts:
  - 分层记忆
  - SOP 固化
  - 原子工具 Agent
related_topics:
  - Agent 框架设计
source_pages:
  - GitHub - GenericAgent
  - Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent
updated: 2026-04-15
---

# 自进化 Agent

## 定义

在这座知识库里，`自进化 Agent` 指的是一种会把已完成任务沉淀成可复用流程、SOP 或 skill 的 agent 设计，而不是每次都从零开始依赖即时上下文。

## 为什么重要

这个概念针对的是普通 agent 的一个老问题：一次会做，不代表下次还会做。只要任务经验不能沉淀，系统就很难形成长期能力积累。自进化路线想解决的，正是“经验如何留存并复用”。

## 关键要点

- 关键不只是“会反思”，而是反思结果能落成后续可调用的结构。
- 这类系统往往会和分层记忆、SOP 固化、最小工具集一起出现。
- GenericAgent 的核心叙事就是：随着使用次数增加，skills 会持续积累，能力树会长出来。
- 这条路线和单纯的会话记忆不同，它强调任务完成后的结构化沉淀。

## 边界

- 它不等于普通的聊天历史记忆。
- 它也不等于“写一份总结文档”就算进化。
- 它容易和插件生态混淆，但这里更强调 agent 自己在执行后沉淀能力，而不是人工安装更多模块。

## 常见分歧

- 有人更看重工具集和运行时能力，认为沉淀机制只是附加值。
- 也有人认为没有能力沉淀的 agent 很难形成真实生产力。
- 目前 GenericAgent 来源明显偏后者，但关于其实际效果和泛化能力，还主要停留在项目自述与团队经验层。

## 关系

- `定义` <- [[GitHub - GenericAgent]]：README 是当前库里对这个概念最稳的定义来源。
- `宣传` <- [[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]]：论坛帖强化了它在社区里的传播标签。
- `属于上位主题` -> [[Agent 框架设计]]：它是当前这组 Agent 框架来源里最核心的设计主张之一。

## 相关来源

- [[GitHub - GenericAgent]]
- [[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]]

## 相关概念

- 分层记忆
- SOP 固化
- 原子工具 Agent

## 相关主题

- [[Agent 框架设计]]
