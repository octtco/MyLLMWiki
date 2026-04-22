---
type: concept
status: active
aliases:
  - Specification
  - 规范层
tags:
  - AI Coding
  - Spec
related_concepts:
  - Skill
related_topics:
  - AI coding framework
source_pages:
  - GitHub - Trellis
  - Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践
updated: 2026-04-22
---

# Spec

## 定义

在这座知识库里，`Spec` 指的是 AI coding 工作流里的稳定约束层。它承载的不是临时任务内容，而是那些跨任务也希望保持稳定的规则，比如项目规范、结构边界、执行要求和上下文约束。

## 它通常接在哪些问题后面

当团队发现“每来一个新任务，就得把同一套规则重讲一遍”时，通常就会需要 `Spec`。它也常和 [[Skill]] 一起出现，因为约束层和能力层解决的不是同一个问题。

## 这页不打算替你解释什么

这页不负责重讲整个 [[AI coding framework]]。它也不负责讨论具体项目里 spec 该怎么分层、怎么注入，这些都要回到对应框架或案例里再说。

## 谁会最常调用它

- [[AI coding framework]] 会拿它解释“为什么框架不等于一堆 prompt 文件”。

## 边界

- `Spec` 不等于一切提示词。
- 它也不等于每次任务临时补的一段说明。
- 只靠 `Spec` 本身，并不能自动补出执行能力。

## 关系

- `相关` -> [[Skill]]：当前来源更支持“约束层”和“能力层”分工协同，而不是互相替代。
- `属于上位主题` -> [[AI coding framework]]：它是当前框架讨论里的核心原子概念之一。
- `定义` <- [[GitHub - Trellis]]：README 给出了最稳定的结构支撑。
- `支持` <- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]：论坛帖更直接解释了为什么团队觉得需要它。

## 相关来源

- [[GitHub - Trellis]]
- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]

## 相关概念

- [[Skill]]

## 相关主题

- [[AI coding framework]]
