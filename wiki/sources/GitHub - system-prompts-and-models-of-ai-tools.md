---
type: source
status: active
source_path: raw/repos/2026-06-10-github-x1xhlol-system-prompts-and-models-of-ai-tools/system-prompts-and-models-of-ai-tools.md
source_type: repo
source_url: https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools
source_bundle: raw/repos/2026-06-10-github-x1xhlol-system-prompts-and-models-of-ai-tools
title: GitHub - system-prompts-and-models-of-ai-tools
authors:
  - x1xhlol
created_at: 2026-06-10
updated_at: 2026-06-10
tags:
  - Prompt
  - Security
  - AI Coding
  - Review
related_methods: []
related_concepts: []
related_topics:
  - 提示词设计
  - AI coding framework
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - system-prompts-and-models-of-ai-tools

## 一句话总结

system-prompts-and-models-of-ai-tools 是一个收集多种 AI 工具 system prompts、internal tools 和模型信息的高关注仓库，当前更适合当作提示词泄露 / AI 产品安全边界样本，而不是复刻或绕过教程。

## 当前范围

本页只整理 README 和 GitHub API 元数据；不展开仓库内具体 prompts、internal tools、提取路径或可复用绕过方法，也不判断其中每份材料的来源合法性和时效真实性。

## 摘要

- GitHub 描述称仓库覆盖 Augment Code、Claude Code、Cursor、Devin、Kiro、Lovable、Manus、Perplexity、Replit、Windsurf、Xcode、v0 等 AI 工具的 system prompts、internal tools 和 AI models 信息。
- README 当前主体内容较短，包含 sponsor、roadmap、feedback、connect 信息，以及面向 AI startups 的 security notice。
- README 明确提醒 exposed prompts or AI models 可能成为攻击目标，并链接到 prompt injection / system prompt extraction 风险相关服务。
- GitHub API 抓取时显示主语言为空，GPL-3.0 license，stars 约 139198，仓库未归档。

## 当前可支持的判断

- 当前来源支持：system prompt / internal tool 信息已经形成高关注公开集合，说明 AI 产品的系统提示词和工具说明会被外部持续收集。
- 当前可保守迁出：它补充 [[提示词设计]] 中“prompt 不只是写作技巧，也可能成为产品安全边界和泄露面”的侧面。
- 它也补充 [[AI coding framework]]：coding agent / AI 工具的 system prompt、internal tools 和模型配置会影响框架行为，但不能把泄露材料当成稳定文档接口。
- 对 [[AI 工具化知识工作流]] 的补充在安全层：工作流产品一旦把 prompts、tools、模型路由暴露出来，就会产生治理和防护问题。

## 当前边界

- 仓库内容高度敏感且时效强，当前不复刻 prompts、不整理提取步骤、不把内部工具名写成可操作清单。
- README 和仓库描述不能证明所有材料来源合法、完整或最新。
- 这类材料适合用于理解 prompt leakage、prompt injection 和 AI 产品安全风险，不适合直接用于模仿、绕过或对抗具体服务。
- 后续若要研究，只应在授权、合规和防御性安全语境下做抽样审查。

## 相关主题

- [[提示词设计]]
- [[AI coding framework]]
- [[AI 工具化知识工作流]]

## 关系

- `待验证` -> [[提示词设计]]：提供 system prompt 作为产品安全边界和泄露面的样本。
- `补充` -> [[AI coding framework]]：提醒 coding agent 的 prompt / tool 层会影响框架行为，但不等于公开 API。
- `补充` -> [[AI 工具化知识工作流]]：提供 AI 工具安全治理样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-10-github-x1xhlol-system-prompts-and-models-of-ai-tools/system-prompts-and-models-of-ai-tools.md](../../raw/repos/2026-06-10-github-x1xhlol-system-prompts-and-models-of-ai-tools/system-prompts-and-models-of-ai-tools.md)
