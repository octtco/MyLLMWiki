---
type: topic
status: active
tags:
  - AI Coding
  - Framework
related_topics:
  - Agent 框架设计
related_concepts:
  - Spec
  - Skill
source_pages:
  - GitHub - Trellis
  - Trellis Doc - 中文文档
  - GitHub - grill-me
  - Linux.do - 大道至简的胜利，一个神级 skill 推荐
  - Linux.do - Trellis + grill-me 组合用起来很爽
  - GitHub - MetaGPT
  - GitHub - awesome-ai-dev-prompts
  - GitHub - awesome-ai-software-development-agents
  - Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践
updated: 2026-05-15
---

# AI coding framework

## 这页真正想回答什么

这页想回答的是：在当前这批来源里，什么样的东西才配叫作 AI coding framework，它和单个规则文件、一次性 prompt、零散脚本到底差在哪里。

## 为什么这个问题很容易讲散

如果只看表面，大家很容易把框架理解成“工具接入很多”“命令很多”或者“目录很多”。但这些都只是外观。真正会把问题讲散的，是没先分清一套框架到底在稳定什么。

## 当前最稳的主线

当前最稳的一条线来自 [[GitHub - Trellis]]、[[Trellis Doc - 中文文档]] 及其配套动机帖：所谓框架，不是把所有内容塞进一个文件里，而是把稳定约束层 [[Spec]]、按需调用的能力层 [[Skill]]、任务层和连续记忆一起组织成可复用工作流。

一旦接受这一点，很多表面分歧就会收束起来。`Spec` 不再是“比 skill 更重要”还是“该被 skill 取代”的问题，而是负责把项目里不该在每次新任务里重讲一遍的东西稳定下来；`Skill` 则负责把任务型能力、特殊工作流和输出纪律以可调用形式留下来。两者不是一套东西，也不是二选一。

## 这条主线是怎样往下走的

先有 [[GitHub - Trellis]] 给出结构定义：`.trellis/spec/`、`.trellis/tasks/`、`.trellis/workspace/` 这些层次本身就在说明，框架关心的是“怎样把规范、任务与连续性放进同一工作面”。

接着，[[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]] 又补了这套结构为什么会被需要：如果项目规范总得反复重讲，或者 skill 总是临场才想起来用，那所谓框架就还没真的站稳。

所以当前更稳的结论不是“Trellis 很强”，而是：在这组来源里，框架的关键价值是让约束、能力、任务和连续性不再各自飘着。

新补进来的 [[GitHub - grill-me]] 和两篇 Linux.do 使用帖，把这条主线往前推了一步：框架接住任务之前，需求本身也要先被问清楚。也就是说，稳定执行不只靠执行时的 task / spec / check，还要靠进入执行前的共享理解。这里更像 [[先追问到共享理解，再进入任务执行]]：先把 plan 或 design 的关键决策分支问到能共同指认，再让 Trellis 这类框架承接后续任务化执行。

再往横向看，[[GitHub - MetaGPT]]、[[GitHub - awesome-ai-dev-prompts]] 和 [[GitHub - awesome-ai-software-development-agents]] 让这页可以多一层边界感：Trellis 这类是框架，`awesome-ai-dev-prompts` 更像 prompt / role prompt 素材库，`awesome-ai-software-development-agents` 更像生态导航表。三者都和 AI coding 有关，但不能混成同一种东西。

## 当前边界

- 这页现在已经补进 `grill-me + Trellis`、MetaGPT、两个 awesome 仓库这些横向样本，但仍不适合过早写成行业通论。
- `best harness`、`没有学习成本` 这类句子仍属于项目方口径。
- `grill-me > brainstorming > plan` 这类排序仍属于社区体验，不适合写成稳定结论。
- prompt 库和 awesome list 只适合当素材层或样本池，不等于已经验证过的框架方法。
- 当前更适合把这页当成“工作定义页”，不是横向优劣排行榜。

## 代表性来源

- [[GitHub - Trellis]]
- [[Trellis Doc - 中文文档]]
- [[GitHub - grill-me]]
- [[Linux.do - 大道至简的胜利，一个神级 skill 推荐]]
- [[Linux.do - Trellis + grill-me 组合用起来很爽]]
- [[GitHub - MetaGPT]]
- [[GitHub - awesome-ai-dev-prompts]]
- [[GitHub - awesome-ai-software-development-agents]]
- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]

## 相关概念

- [[Spec]]
- [[Skill]]

## 相关方法

- [[先追问到共享理解，再进入任务执行]]

## 相关主题

- [[Agent 框架设计]]
