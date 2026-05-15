---
type: source
status: active
source_path: raw/repos/2026-05-15-github-mattpocock-skills-grill-me/grill-me.md
source_type: repo
source_url: https://github.com/mattpocock/skills/blob/main/skills/grill-me/SKILL.md
source_bundle: raw/repos/2026-05-15-github-mattpocock-skills-grill-me
title: GitHub - grill-me
authors:
  - mattpocock
created_at: 2026-05-15
updated_at: 2026-05-15
tags:
  - AI Coding
  - Skill
  - Requirement Clarification
related_methods:
  - 先追问到共享理解，再进入任务执行
related_concepts:
  - Skill
related_topics:
  - AI coding framework
related_cases: []
related_relations: []
---

# GitHub - grill-me

## 一句话总结

`grill-me` 是一个极小的前置澄清型 skill：它不负责直接执行任务，而是先把 plan 或 design 里的决策分支追问到共享理解。

## 当前范围

本页只整理 `skills/grill-me/SKILL.md` 这一个 skill 文件，不整理整个 `mattpocock/skills` 仓库。

## 摘要

- 这个 skill 的核心不是产出长计划，而是连续追问。
- 它把追问目标定义为 shared understanding，而不是“问够问题”本身。
- 它要求沿着 decision tree 处理分支和依赖。
- 它要求一次只问一个问题，避免一次性把用户压进大问卷。
- 它还把“能通过代码库探索回答的问题”交给代码库探索，而不是全部转嫁给用户。

## 证据或原文线索

- GitHub 文件：`skills/grill-me/SKILL.md`
- 关键结构：frontmatter 描述使用场景，正文只有少量执行指令。

## 当前可支持的判断

- 当前来源支持：`Skill` 可以非常小，只要它稳定封装了一个高价值动作。
- 当前来源支持：有些 skill 的主要价值不在执行，而在执行前修掉需求不清和决策依赖未展开的问题。

## 当前边界

- 这份来源不证明 `grill-me` 在所有计划场景都优于更重的 brainstorming。
- 它本身没有规定追问结束后的落盘格式，所以仍需要和计划文档、任务系统或 Trellis 这类后续执行框架配合。

## 相关概念

- [[Skill]]

## 相关方法

- [[先追问到共享理解，再进入任务执行]]

## 相关主题

- [[AI coding framework]]

## 关系

- `定义` -> [[Skill]]：提供一个极简 skill 也能成立的样本。
- `支持` -> [[先追问到共享理解，再进入任务执行]]：直接支撑前置澄清动作。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-15-github-mattpocock-skills-grill-me/grill-me.md](../../raw/repos/2026-05-15-github-mattpocock-skills-grill-me/grill-me.md)
