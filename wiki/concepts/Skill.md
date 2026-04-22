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
source_pages:
  - GitHub - Trellis
  - Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践
  - GitHub - GenericAgent
  - GitHub - anti-default-output
updated: 2026-04-22
---

# Skill

## 定义

在这座知识库里，`Skill` 指的是 AI 系统中可按需调用的能力层。它承载的是任务型能力、工作流经验、工具使用模式，或者某种需要被反复调用的输出纪律。

## 它通常接在哪些问题后面

如果一个系统总是“会做一次，但下次还得重新教”，那通常就会用到 `Skill`。它既可以是完成任务的能力，也可以像 [[反默认输出]] 这样，承担对输出路径的纠偏。

## 这页不打算替你解释什么

这页不负责重讲具体框架，也不负责替某个项目决定 skill 应该放在哪个目录、怎样触发。它只保留最小共享定义。

## 谁会最常调用它

- [[AI coding framework]] 会用它解释为什么框架需要能力层。
- [[Agent 框架设计]] 会用它解释为什么“经验沉淀”是框架设计问题，不只是使用习惯问题。

## 边界

- `Skill` 不等于插件数量。
- 它也不等于普通聊天记忆。
- 它不一定只负责“加新能力”，也可能负责减少默认错误。

## 关系

- `相关` -> [[Spec]]：当前来源更支持二者分工协同。
- `相关` -> [[自进化 Agent]]：在这条设计路线里，任务经验的主要落点就是 skill。
- `相关` -> [[反默认输出]]：有些 skill 的作用不是扩能力，而是纠偏输出惯性。
- `相关` -> [[默认路径]]：某些 skill 会把“识别默认解”本身做成稳定能力。
- `相关` -> [[输出前自检]]：某些 skill 会把生成前检查写成固定动作。

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

## 相关主题

- [[AI coding framework]]
- [[Agent 框架设计]]
