---
type: source
status: review
source_path: raw/web/2026-04-14-linuxdo-topic-1539636-trellis-best-practice/trellis-best-practice.md
source_type: web
source_url: https://linux.do/t/topic/1539636
source_bundle: raw/web/2026-04-14-linuxdo-topic-1539636-trellis-best-practice
title: Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践
authors: []
created_at: 2026-04-22
updated_at: 2026-04-22
tags:
  - AI Coding
  - Framework
  - Trellis
  - Community
related_concepts:
  - Spec
  - Skill
related_topics:
  - AI coding framework
related_relations: []
---

# Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践

## 一句话总结

这是一篇 Trellis 的设计动机帖：它最有价值的地方不是功能清单，而是把作者为什么觉得 `Spec` 和 `Skill` 必须同时存在说得很清楚。

## 摘要

- 帖子先回顾 OpenSpec、plan-with-files、Superpowers 等实践痛点，再引出 Trellis 的设计路线。
- 作者把核心问题收成两件事：项目规范总得反复重写，以及 skill 在复杂项目里调用不稳定。
- 在这个判断上，帖子提出 `Spec 负责约束，Skill 负责能力`，并把自动上下文注入、任务系统和并行 worktree 接到这条线上。

## 证据或原文线索

- `我们踩过的坑` 一节明确指出了 `PRD-driven` 与宽泛 skill 的两个问题。
- `我们的思考` 一节直接写出 `Spec 负责约束`、`Skill 负责能力`。
- `Trellis：为 AI 编码提供结构化支撑` 一节补了分层和索引、自动注入上下文、Todo/Task 系统以及 multi-agent/worktree。

## 我的判断

- 这份来源适合和 [[GitHub - Trellis]] 配对使用，作为框架设计动机的来源。
- 它能够增强 [[Spec]]、[[Skill]] 和 [[AI coding framework]] 这三个节点之间的连接。
- 但帖子里的 `没有学习成本`、`所有复杂逻辑都已经做在框架内部` 这类说法仍属于项目方宣传口径。

## 相关概念

- [[Spec]]
- [[Skill]]

## 相关主题

- [[AI coding framework]]

## 关系

- `支持` -> [[Spec]]：这篇帖子更直接解释了为什么团队觉得需要一个稳定约束层。
- `支持` -> [[Skill]]：这篇帖子更直接解释了为什么能力层不能只靠临时 prompt。
- `补充` -> [[GitHub - Trellis]]：README 讲结构，这篇帖子讲为什么会长成这种结构。

## 回链

- 对应来源包主文件：[raw/web/2026-04-14-linuxdo-topic-1539636-trellis-best-practice/trellis-best-practice.md](../../raw/web/2026-04-14-linuxdo-topic-1539636-trellis-best-practice/trellis-best-practice.md)
