---
type: concept
status: active
aliases:
  - Self-Evolving Agent
tags:
  - Agent
  - Memory
  - Skill
related_concepts:
  - Skill
related_topics:
  - Agent 框架设计
source_pages:
  - GitHub - GenericAgent
  - Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent
updated: 2026-04-22
---

# 自进化 Agent

## 定义

在这座知识库里，`自进化 Agent` 指的是一种会把已完成任务沉淀成可复用 skill、SOP 或结构化经验的 agent 设计，而不是每次都从零开始依赖当场上下文。

## 它通常接在哪些问题后面

普通 agent 的一个老问题是：这次会做，不代表下次还会做。只要任务经验不能留存，系统就很难形成长期能力积累。`自进化 Agent` 想解决的正是这一点。

## 这页不打算替你解释什么

这页不负责证明 GenericAgent 的所有宣传性能力，也不负责重讲整个框架结构。它只保留“经验如何沉淀并复用”这条共享定义。

## 谁会最常调用它

- [[Agent 框架设计]] 会用它来说明，为什么长期能力积累本身就是框架设计问题。

## 边界

- 它不等于普通会话记忆。
- 它也不等于写一份总结就算进化。
- 它和插件生态有关，但不是一回事。

## 关系

- `相关` -> [[Skill]]：任务后的沉淀结果通常落成可复用 skill。
- `属于上位主题` -> [[Agent 框架设计]]：它是当前这组来源里最稳的设计抓手之一。
- `定义` <- [[GitHub - GenericAgent]]：README 给出了最稳定的定义来源。
- `宣传` <- [[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]]：论坛帖强化了它在社区里的传播标签。

## 相关来源

- [[GitHub - GenericAgent]]
- [[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]]

## 相关概念

- [[Skill]]

## 相关主题

- [[Agent 框架设计]]
