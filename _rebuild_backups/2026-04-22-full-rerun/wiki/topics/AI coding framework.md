---
type: topic
status: active
tags:
  - AI Coding
  - Framework
  - Trellis
related_topics:
  - Agent 框架设计
related_concepts:
  - Spec
  - Skill
source_pages:
  - GitHub - Trellis
  - Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践
updated: 2026-04-15
---

# AI coding framework

## 问题定义

这一页想回答：在当前这批来源里，什么样的结构才配叫作 AI coding framework，它和单纯的规则文件、单次 agent 提示或零散脚本有什么区别。

## 当前结论

目前这组来源更支持一种“工作流层框架”理解：AI coding framework 的核心不是单个模型或单个 agent，而是把 spec、task、memory、平台接入和协作流程组织成一个可复用系统。Trellis 是当前库里最能直接支撑这一定义的样本。就当前材料看，更稳的表达是把 [[Spec]] 和 [[Skill]] 视为两个原子概念，再讨论它们的分工关系。

## 主要脉络

- [[GitHub - Trellis]] 提供了更稳定的结构定义，明确把 `.trellis/`、spec、tasks、workspace memory 和多平台接入放进同一套结构。
- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]] 补的是设计动机：为什么团队会觉得只靠单规则文件或单层 prompt 不够。
- [[Spec]] 和 [[Skill]] 是当前最稳的两个原子概念，前者偏约束层，后者偏能力层。
- 现阶段这个主题还主要由 Trellis 相关来源支撑，所以更适合当“工作定义页”，不宜过早写成通用行业结论。

## 代表性来源

- [[GitHub - Trellis]]
- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]

## 还不清楚的地方

- 现在还缺更多框架对照来源，暂时不适合做横向优劣判断。
- “best harness”“几乎没有学习成本”这类表述仍主要是项目方口径。
- 还没有足够材料支撑更强关系，比如“某类框架普遍优于另一类框架”。

## 后续可追的问题

- 补更多 AI coding framework 样本，增强横向比较能力。
- 补 `Spec 注入`、`Task-centered workflow`、`Project memory` 等二级概念页。
- 继续观察 Trellis 之外的项目是否也支持 Spec/Skill 分工这条路线。

## 相关概念

- [[Spec]]
- [[Skill]]

## 相关主题

- [[Agent 框架设计]]
