---
type: concept
status: active
aliases:
  - Specification
  - 规范层
tags:
  - AI Coding
  - Spec
  - Trellis
related_concepts:
  - Skill
  - Spec 注入
  - Task-centered workflow
related_topics:
  - AI coding framework
source_pages:
  - GitHub - Trellis
  - Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践
updated: 2026-04-15
---

# Spec

## 定义

在这座知识库里，`Spec` 指的是 AI coding 工作流里的稳定约束层，用来承载项目级规则、结构边界、执行要求和上下文约束。

## 为什么重要

如果没有 Spec，AI 在跨任务、跨会话、跨人协作时就容易失去稳定边界。Spec 的价值不在于“写得很多”，而在于把那些必须稳定存在的约束从临时 prompt 里抽出来。

## 关键要点

- `Spec` 更适合承载风格、目录规则、架构边界、错误处理、约束条件。
- 它强调的是稳定性和可预测性，而不是灵活应变。
- 在 Trellis 相关来源里，Spec 往往不是单个文件，而是一个分层、可注入、可复用的约束系统。

## 边界

- 它不等于一切提示词。
- 它也不等于临时任务说明。
- 只靠 Spec 并不能自动补齐执行能力。

## 常见分歧

- 一种做法倾向把更多能力都写进规范里，希望靠规则覆盖执行问题。
- 另一种做法认为 Spec 只该保留稳定约束，能力层应交给 Skill。
- 当前 Trellis 来源更支持后者。

## 关系

- `相关` -> [[Skill]]：当前来源更支持“约束层”和“能力层”协同，而不是互相替代。
- `属于上位主题` -> [[AI coding framework]]：它是当前工作流框架讨论中的核心原子概念之一。
- `定义` <- [[GitHub - Trellis]]：README 提供了更稳定的结构支撑。
- `支持` <- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]：论坛帖补了为什么需要 Spec 层。

## 相关来源

- [[GitHub - Trellis]]
- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]

## 相关概念

- [[Skill]]
- Spec 注入
- Task-centered workflow

## 相关主题

- [[AI coding framework]]
