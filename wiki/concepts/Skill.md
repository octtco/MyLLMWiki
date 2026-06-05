---
type: concept
status: active
aliases:
  - 能力层
  - Task Skill
tags:
  - AI Coding
  - Skill
related_concepts:
  - Spec
  - 自进化 Agent
  - 反默认输出
  - 默认路径
  - 输出前自检
related_topics:
  - AI coding framework
  - Agent 框架设计
  - 提示词设计
source_pages:
  - GitHub - Trellis
  - GitHub - grill-me
  - Trellis Doc - 中文文档
  - Linux.do - 大道至简的胜利，一个神级 skill 推荐
  - Linux.do - Trellis + grill-me 组合用起来很爽
  - GitHub - awesome-ai-dev-prompts
  - Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践
  - GitHub - GenericAgent
  - GitHub - anti-default-output
  - The Prompting Book
updated: 2026-05-25
---

# Skill

## 定义

在这座知识库里，`Skill` 指的是 AI 系统中可按需调用的能力层。它承载的是任务型能力、工作流经验、工具使用模式，或者某种需要被反复调用的输出纪律。

## 它通常接在哪些问题后面

如果一个系统总是“会做一次，但下次还得重新教”，那通常就会用到 `Skill`。它既可以是完成任务的能力，也可以像 [[反默认输出]] 这样，承担对输出路径的纠偏。

这次补进来的 [[GitHub - grill-me]] 说明，`Skill` 也可以承载执行前的澄清纪律：它不直接写代码，也不负责完整计划，而是把追问、分支决策和共享理解做成一个可调用动作。

[[GitHub - awesome-ai-dev-prompts]] 则提供了一个边界样本：prompt 库和 skill 相邻，但不完全相同。prompt 更像可复制的文本素材；skill 通常还需要触发时机、上下文约束、工具动作和验收纪律。

[[The Prompting Book]] 进一步补了这个边界：它把 prompts、skills、agents 写成从基础材料到复合结构的关系。这个比喻当前可以低强度复用，但不能把所有 skill 都还原成 prompt 拼装；仓库里仍然把触发条件、上下文纪律和验收要求看成 skill 的关键部分。

## 这页不打算替你解释什么

这页不负责重讲具体框架，也不负责替某个项目决定 skill 应该放在哪个目录、怎样触发。它只保留最小共享定义。

## 谁会最常调用它

- [[AI coding framework]] 会用它解释为什么框架需要能力层。
- [[Agent 框架设计]] 会用它解释为什么“经验沉淀”是框架设计问题，不只是使用习惯问题。

## 边界

- `Skill` 不等于插件数量。
- 它也不等于普通聊天记忆。
- 它不一定只负责“加新能力”，也可能负责减少默认错误。
- 它不一定只发生在执行阶段，也可能先发生在任务进入框架之前。
- 它也不等于 prompt 收藏夹；只有当文本能力被放进可调用流程和执行纪律里，才更接近 skill。

## 关系

- `相关` -> [[Spec]]：当前来源更支持二者分工协同。
- `相关` -> [[自进化 Agent]]：在这条设计路线里，任务经验的主要落点就是 skill。
- `相关` -> [[反默认输出]]：有些 skill 的作用不是扩能力，而是纠偏输出惯性。
- `相关` -> [[默认路径]]：某些 skill 会把“识别默认解”本身做成稳定能力。
- `相关` -> [[输出前自检]]：某些 skill 会把生成前检查写成固定动作。
- `相关` -> [[先追问到共享理解，再进入任务执行]]：某些 skill 的价值是先把需求和设计分支问清楚。

## 相关来源

- [[GitHub - Trellis]]
- [[GitHub - grill-me]]
- [[Trellis Doc - 中文文档]]
- [[Linux.do - 大道至简的胜利，一个神级 skill 推荐]]
- [[Linux.do - Trellis + grill-me 组合用起来很爽]]
- [[GitHub - awesome-ai-dev-prompts]]
- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]
- [[GitHub - GenericAgent]]
- [[GitHub - anti-default-output]]
- [[The Prompting Book]]

## 相关概念

- [[Spec]]
- [[自进化 Agent]]
- [[反默认输出]]
- [[默认路径]]
- [[输出前自检]]

## 相关主题

- [[AI coding framework]]
- [[Agent 框架设计]]
- [[提示词设计]]
