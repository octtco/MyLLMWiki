---
type: concept
status: active
aliases:
  - 能力层
  - Task Skill
tags:
  - AI Coding
  - Skill
  - Trellis
  - GenericAgent
  - anti-default-output
related_concepts:
  - Spec
  - 自进化 Agent
  - 反默认输出
  - 默认路径
  - 输出前自检
  - SOP 固化
related_topics:
  - AI coding framework
  - Agent 框架设计
source_pages:
  - GitHub - Trellis
  - Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践
  - GitHub - GenericAgent
  - GitHub - anti-default-output
updated: 2026-04-16
---

# Skill

## 定义

在这座知识库里，`Skill` 指的是 AI 系统中可按需调用的能力层，用来承载特定工作流、上下文注入方式、工具使用模式和任务型执行经验。

## 为什么重要

如果所有能力都只能靠即时 prompt 现场拼接，系统就很难形成长期复用。Skill 的意义，是把“会做一次”变成“以后还能稳定再做”。

## 关键要点

- Skill 更适合承载任务型能力，而不是项目级硬约束。
- 它经常和 SOP、工作流模板、工具调用习惯、上下文注入一起出现。
- 在 GenericAgent 相关来源里，任务后沉淀 skill / SOP 是很核心的叙事。
- 在 Trellis 相关来源里，Skill 更接近能力扩展层，与 Spec 分工配合。
- 在 anti-default-output 这类来源里，Skill 还可以是“输出纠偏层”，专门用来矫正模型滑向默认生成路径的倾向。
- 这类纠偏型 skill 往往还会把 [[默认路径]] 的识别和 [[输出前自检]] 的动作一起封装进去。

## 边界

- 它不等于插件市场或模块数量。
- 它也不等于普通聊天记忆。
- 它不一定只负责“加能力”，也可以负责“纠偏输出路径”。
- Skill 如果没有约束层配合，容易灵活但不稳定。

## 常见分歧

- 一种做法把 Skill 当成功能增强件，认为它只是附加值。
- 另一种做法认为没有 Skill 沉淀，就难形成长期复用能力。
- 还有一种做法会把 Skill 当成生成纪律的封装，不是加新功能，而是减少默认错误和模板化输出。
- 当前 GenericAgent 和 Trellis 来源都更支持“Skill 是核心层之一”，只是侧重点不同。

## 关系

- `相关` -> [[Spec]]：当前来源更支持二者分工协同，而不是由其中一方完全替代另一方。
- `相关` -> [[自进化 Agent]]：自进化路线里，Skill 往往是任务经验沉淀后的主要落点。
- `相关` -> [[反默认输出]]：有些 skill 的价值不在扩能力，而在纠偏默认生成路径。
- `相关` -> [[默认路径]]：有些 skill 会把“识别默认生成惯性”本身做成稳定能力。
- `相关` -> [[输出前自检]]：有些 skill 不只给结果要求，还会规定生成前必须先做的检查动作。
- `属于上位主题` -> [[AI coding framework]]：它是当前工作流框架讨论中的核心原子概念之一。
- `属于上位主题` -> [[Agent 框架设计]]：在 Agent 框架来源里，Skill 沉淀也是重要设计抓手。

## 相关来源

- [[GitHub - Trellis]]
- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]
- [[GitHub - GenericAgent]]
- [[GitHub - anti-default-output]]

## 相关概念

- [[Spec]]
- [[自进化 Agent]]
- [[反默认输出]]
- [[默认路径]]
- [[输出前自检]]
- SOP 固化

## 相关主题

- [[AI coding framework]]
- [[Agent 框架设计]]
