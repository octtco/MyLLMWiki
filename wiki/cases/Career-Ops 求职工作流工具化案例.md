---
type: case
status: review
case_type: 来源内案例
tags:
  - Career
  - Automation
  - Claude Code
related_topics:
  - AI 工具化知识工作流
related_methods: []
related_concepts:
  - Skill
related_cases: []
source_pages:
  - GitHub - Career-Ops
updated: 2026-06-09
---

# Career-Ops 求职工作流工具化案例

## 具体对象

这个案例的对象是 [[GitHub - Career-Ops]]：一个基于 Claude Code 的 AI 求职系统样本。

## 具体场景

求职不是单次文本生成任务，而是一组连续动作：理解个人 CV、筛选目标岗位、分析公司、生成简历或材料、批量处理机会、追踪进度，并在真实性、隐私和平台规则之间保持边界。

这个场景很适合观察 AI 知识工作流何时从“帮我写一段话”变成“把一组职业动作组织成工具化流程”。

## 具体过程

Career-Ops 的 README 把系统组织成 skill modes、dashboard、PDF generation 和 batch processing。Quick Start 要求先准备 `cv.md`，再让 Claude 基于个人 CV、目标角色、公司列表和语言偏好定制工作流。

也就是说，它不是只收藏一堆求职 prompt，而是把求职材料、岗位分析、输出格式和批处理放进一套可调用流程里。这里的 [[Skill]] 更像工作流能力单元：不同求职动作被模式化后，才有机会反复调用。

## 这个案例说明了什么

这个案例支撑 [[AI 工具化知识工作流]]：知识工作流的工具化不是只让模型生成文本，而是把输入材料、任务模式、输出产物和执行界面一起组织起来。

它同时提醒：越接近真实外部平台和个人身份，越不能只看效率。求职自动化天然涉及个人隐私、真实性、招聘公平性和平台条款，必须以 `review` 口径保留。

## 边界

- 当前未安装 Career-Ops，也未测试 dashboard、PDF、batch processing 或 Gemini CLI integration。
- 当前不迁出自动投递步骤，不把 README 口径写成可直接执行的求职自动化建议。
- 简历生成和岗位匹配必须人工审核，不能默认批量生成就是合适材料。

## 相关来源

- [[GitHub - Career-Ops]]

## 相关主题

- [[AI 工具化知识工作流]]

## 相关方法

- 暂无

## 相关概念

- [[Skill]]

## 相关案例

- 暂无
