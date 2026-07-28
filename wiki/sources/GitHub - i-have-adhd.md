---
type: source
status: review
source_path: raw/repos/2026-07-24-github-ayghri-i-have-adhd/README.md
source_type: repo
source_url: https://github.com/ayghri/i-have-adhd
source_bundle: raw/repos/2026-07-24-github-ayghri-i-have-adhd
title: GitHub - i-have-adhd
authors:
  - ayghri
created_at: 2026-07-24
updated_at: 2026-07-24
tags:
  - AI Coding
  - Skill
  - Output Format
related_methods: []
related_concepts:
  - Skill
related_topics:
  - AI coding framework
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - i-have-adhd

## 一句话总结

这是一个给 Claude Code、Codex 等 coding agent 使用的 ADHD-friendly 输出风格 skill，用可检查的格式规则减少答案埋藏、无关发散和执行步骤不清。

## 当前范围

本轮依据官方 README 整理。已确认项目的定位、Claude Code / Codex 安装入口、十条输出规则和 MIT 许可；没有安装 skill，也没有验证不同模型对规则的长期遵守程度。

## 摘要

- 它要求回答先给下一步行动，多步骤任务使用编号，并在结尾留下一个具体下一步。
- 它要求每轮重述当前状态、限制列表长度、压制切题外内容，并用事实化语气表达错误。
- 它把“ADHD-friendly”用于 coding agent 的信息组织，不是 ADHD 诊断工具，也不是人类日程管理应用。
- 它可以作为 Claude Code / Codex 插件安装，也可以 fork 后修改自己的 `SKILL.md`。
- 它的核心价值在于把“请简洁一点”变成一组可以直接注入 agent 的行为约束。

## 证据或原文线索

- README 将项目定位为让 coding assistant 不再把答案埋在长篇铺垫里。
- 安装说明同时覆盖 Claude Code 和 Codex，并提供显式调用方式。
- 十条规则包含“先给行动”“步骤编号”“每轮重述状态”“列表最多五项”和“只留一个下一步”等约束。
- README 明确说明灵感来自 *The Adult ADHD Tool Kit*，但适配对象是 LLM 的回答方式，而不是人的日程组织。

## 当前可支持的判断

- 这是一个输出纪律 skill，不是新的模型、agent runtime 或任务执行器。
- 它与 [[Skill]] 的关系是：把一组可复用的输出行为约束打包成可安装能力。
- 它与 [[AI coding framework]] 的关系是：提供轻量的交互 / 表达约束，但不能独立构成完整框架。
- 它与 [[AI 工具化知识工作流]] 的关系是：把回答组织方式从个人偏好变成可复用的工作流资产。

## 当前边界

- 规则可能与需要完整解释、正式文档或高风险确认的任务发生张力，不能机械地把所有回答压缩成短句。
- skill 只能增加模型遵守某种输出风格的机会，不能保证模型始终遵守，也不能保证答案正确。
- 本轮没有分别保存仓库内的核心 `SKILL.md`，因此暂不对其完整实现细节、触发逻辑或其他 host 的适配作强结论。
- “ADHD-friendly”是项目的产品命名和设计取向，不应被写成医学效果或临床建议。

## 相关概念

- [[Skill]]

## 相关主题

- [[AI coding framework]]
- [[AI 工具化知识工作流]]

## 关系

- `体现` -> [[Skill]]：把输出纪律组织为可安装、可 fork 的 agent skill。
- `补充` -> [[AI coding framework]]：为框架增加交互结构和输出可扫读性的轻量约束。
- `支持` -> [[AI 工具化知识工作流]]：把“如何回答”从临时偏好转成可复用工具资产。

## 回链

- 对应来源包主文件：[raw/repos/2026-07-24-github-ayghri-i-have-adhd/README.md](../../raw/repos/2026-07-24-github-ayghri-i-have-adhd/README.md)
