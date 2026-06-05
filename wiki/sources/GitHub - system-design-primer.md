---
type: source
status: review
source_path: raw/repos/2026-05-28-github-donnemartin-system-design-primer/system-design-primer.md
source_type: repo
source_url: https://github.com/donnemartin/system-design-primer
source_bundle: raw/repos/2026-05-28-github-donnemartin-system-design-primer
title: GitHub - system-design-primer
authors:
  - donnemartin
created_at: 2026-05-28
updated_at: 2026-05-28
tags:
  - System Design
  - Learning
  - Interview
related_methods: []
related_concepts: []
related_topics:
  - 系统设计学习入口
related_cases: []
related_relations: []
---

# GitHub - system-design-primer

## 一句话总结

system-design-primer 是一个系统设计学习和面试准备入口，把分散的可扩展系统主题、练习题、案例解法和记忆卡组织到一条学习路线里。

## 当前范围

本页只整理 README 主干，不读取 `solutions/` 细节，不验证所有外链，也不把仓库里的系统设计结论全部拆成概念页。

## 摘要

- README 把目标分成两块：学习大规模系统设计，以及准备系统设计面试。
- 仓库强调 system design 资源分散，因此它提供一个 organized collection。
- 主题索引覆盖 performance/scalability、latency/throughput、availability/consistency、CAP、consistency patterns、availability patterns、DNS、CDN、load balancer、database、cache、asynchronism、communication、security 等。
- 学习建议按 short / medium / long timeline 区分，强调先广度，再按时间和经验补深度。
- 面试过程被拆成四步：列 use cases / constraints / assumptions，画 high level design，深入 core components，再根据瓶颈 scale design。
- 仓库还包含系统设计和 OOD 面试题解，以及 Anki flashcards。

## 证据或原文线索

- GitHub API 抓取时显示 license 为 `NOASSERTION`，stars 约 350.6k，仓库未归档。
- README heading 包括 `Motivation`、`Index of system design topics`、`Study guide`、`How to approach a system design interview question`、`System design interview questions with solutions`。
- README 明确写到 `Everything is a trade-off`，并在主题入口里把 trade-off 放在中心位置。

## 当前可支持的判断

- 当前来源支持：系统设计学习最容易散成技术名词表，而这个仓库的价值在于把基础主题、权衡框架和面试表达过程放到同一入口。
- 当前可保守迁出：面试型系统设计训练需要同时练“知道组件”和“按约束讲出取舍”。

## 当前边界

- README 很长，本轮没有展开所有章节和解法。
- 不把 interview prep 写成真实工程设计能力的充分证明。
- license 字段为 `NOASSERTION`，复用材料前需要继续看仓库许可文件和内容来源。

## 相关主题

- [[系统设计学习入口]]

## 关系

- `支持` -> [[系统设计学习入口]]：提供系统设计学习路径和面试过程样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-28-github-donnemartin-system-design-primer/system-design-primer.md](../../raw/repos/2026-05-28-github-donnemartin-system-design-primer/system-design-primer.md)

