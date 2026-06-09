---
type: source
status: review
source_path: raw/books/2026-05-25-prompts-chat-the-prompting-book/README.md
source_type: book
source_url: https://prompts.chat/book
source_bundle: raw/books/2026-05-25-prompts-chat-the-prompting-book
title: The Prompting Book
authors:
  - Fatih Kadir Akin
year: 2025
created_at: 2026-05-25
updated_at: 2026-05-25
tags:
  - Prompt
  - Prompt Engineering
  - LLM
related_methods: []
related_concepts:
  - Skill
related_topics:
  - 提示词设计
  - AI 工具化知识工作流
  - AI coding framework
related_cases: []
related_relations:
  - Prompt - 组织为 - Skill
---

# The Prompting Book

## 一句话总结

`The Prompting Book` 把提示词从零散技巧整理成一条从基础构件、常用技术、上下文工程到 agents / skills 的实践链。

## 当前范围

本轮只整理中英两版 PDF 的目录骨架、章节主线和可迁出的低强度判断。全书逐章细读、示例效果验证、方法页拆分先留在工作层。

## 摘要

- 这本书来自 prompts.chat / Awesome ChatGPT Prompts 生态，作者把它定位为新版提示词实践指南。
- 基础部分强调先理解模型与 prompt 构件，再系统组合 role、context、task、constraints、format、examples 和 tone。
- 技巧部分覆盖角色提示、结构化输出、思维链、few-shot、迭代改进、JSON/YAML 等常用做法。
- 高阶部分把单条 prompt 推向 system prompt、prompt chaining、edge cases、多模态、context engineering、agents 与 skills。
- 最适合当前知识库吸收的不是“最佳 prompt 清单”，而是提示词设计如何逐步接近可复用工作流。

## 证据或原文线索

- 英文 PDF 目录显示全书包含 `Foundations`、`Techniques`、`Advanced Strategies`、`Best Practices`、`Use Cases` 和 `Conclusion`。
- `Anatomy of an Effective Prompt` 章节把有效 prompt 拆成 role、context、task、constraints、format、examples、tone 等构件。
- `Context Engineering` 章节强调模型无状态，必须把正确上下文在正确时间提供给模型。
- `Agents & Skills` 章节把 prompts、skills、agents 组织成从原子到组合结构的关系。

## 当前可支持的判断

- 当前来源支持：提示词设计可以被看成一组可拆解、可迭代、可接入工作流的沟通结构，而不是只靠灵感写“神词”。
- 当前可保守迁出：prompt library 是素材层，prompt chaining、context engineering、skills 和 agents 则把素材推进到系统层。
- 当前适合回写：[[提示词设计]]、[[AI 工具化知识工作流]]、[[AI coding framework]] 和 [[Skill]]。

## 当前边界

- 不把书中技巧写成对所有模型永远有效的标准。
- 不把 CoT、few-shot、JSON/YAML 这类章节自动升成概念页。
- 不把 use case 章节里的场景描述直接当作正式案例页。
- 不用单书来源证明某种 prompt 写法在生产环境稳定。

## 相关概念

- [[Skill]]

## 相关主题

- [[提示词设计]]
- [[AI 工具化知识工作流]]
- [[AI coding framework]]

## 关系

- `支持` -> [[提示词设计]]：提供提示词构件、技巧、上下文工程和应用层的完整目录骨架。
- `补充` -> [[AI 工具化知识工作流]]：把 prompt 资产化和工具化之间的中间层讲得更清楚。
- `补充` -> [[Skill]]：提供 `prompts -> skills -> agents` 的低强度结构比喻。

## 回链

- 对应来源包：[raw/books/2026-05-25-prompts-chat-the-prompting-book/README.md](../../raw/books/2026-05-25-prompts-chat-the-prompting-book/README.md)
- 长书工作层：[outputs/reports/2026-05-25-The-Prompting-Book-长书拆解工作层/00-范围与骨架.md](../../outputs/reports/2026-05-25-The-Prompting-Book-长书拆解工作层/00-范围与骨架.md)
