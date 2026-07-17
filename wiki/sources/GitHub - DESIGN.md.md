---
type: source
status: review
source_path: raw/repos/2026-07-14-github-google-labs-code-design-md/README.md
source_type: repo
source_url: https://github.com/google-labs-code/design.md
source_bundle: raw/repos/2026-07-14-github-google-labs-code-design-md
title: GitHub - DESIGN.md
authors:
  - Google Labs Code
created_at: 2026-07-14
updated_at: 2026-07-14
tags:
  - Design System
  - AI Coding
  - Design Tokens
  - CLI
related_methods: []
related_concepts:
  - Spec
related_topics:
  - 设计系统与平台规范
  - AI coding framework
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - DESIGN.md

## 一句话总结

这是一个面向 coding agent 的设计规范格式，以及围绕该格式提供校验、比较、导出和规范输出的 TypeScript CLI 工具链。

## 当前范围

本轮依据官方 README 和 GitHub API 元数据整理。已确认仓库定位、文件格式、CLI 命令和 alpha 状态；没有安装 CLI，也没有验证 agent 在真实项目中对 DESIGN.md 的遵守程度。

## 摘要

- `DESIGN.md` 由 YAML front matter 和 Markdown 正文两层组成：前者保存机器可读的设计 tokens，后者解释设计理由和使用语境。
- 规范覆盖颜色、字体、间距、圆角、组件 token、章节顺序和 Do's / Don'ts 等内容。
- `lint` 命令可以检查 token 引用、颜色对比度、孤立 token、字体缺失、章节顺序和疑似拼写错误。
- `diff` 命令可以比较两个 DESIGN.md 版本，报告 token 变更和潜在回归。
- `export` 可以将设计 token 导出成 Tailwind 配置、Tailwind CSS、DTCG 等格式。
- `spec` 可以输出格式规范，方便把规范上下文注入 coding agent 的提示或工作流。
- 仓库同时提供程序化 API，能够在其他工具中调用 linter；当前格式仍处于 alpha 阶段。

## 证据或原文线索

- README 将项目定义为“描述 visual identity 给 coding agents 的 format specification”。
- 示例中的 `DESIGN.md` 以 `colors`、`typography`、`rounded` 和 `spacing` token 描述一个具体设计系统。
- README 明确给出 `npx @google/design.md lint DESIGN.md`、`diff`、`export` 和 `spec` 命令。
- lint 规则包含 `broken-ref`、`contrast-ratio`、`orphaned-tokens`、`missing-typography` 和 `section-order` 等检查。

## 当前可支持的判断

- 它的核心不是“自动生成一套好看的 design”，而是定义一种让人和 coding agent 共享设计约束的文件格式。
- 它把设计系统从只存在于 Figma、口头经验或散落 CSS 中的东西，部分转成可版本控制、可检查、可导出的项目资产。
- 它比单纯的 Markdown 模板更完整，因为仓库还提供围绕格式运行的 CLI 和程序化 API。
- 它能提高 agent 获取设计上下文和保持 token 一致性的机会，但不能强制模型遵守设计，也不能证明最终页面一定好看。

## 当前边界

- `DESIGN.md` 格式当前标记为 alpha，schema、token 规则和 CLI 行为仍可能变化。
- README 只说明规范和工具能力，本轮没有跑 `lint`、`diff` 或 `export`，也没有验证真实前端项目效果。
- 工具主要验证 DESIGN.md 和 token 层，不等于对最终网页截图、交互质量或品牌一致性做完整验收。
- 仓库没有把现有 Figma、截图或任意设计自动转换成 DESIGN.md 的能力说明；设计内容仍需要人工或其他 agent 先整理出来。

## 相关概念

- [[Spec]]

## 相关主题

- [[设计系统与平台规范]]
- [[AI coding framework]]
- [[AI 工具化知识工作流]]

## 关系

- `体现` -> [[Spec]]：把设计约束组织成可被工具读取和校验的规范文件。
- `补充` -> [[设计系统与平台规范]]：把传统设计系统和平台规范接到 coding agent 可消费的文件层。
- `补充` -> [[AI coding framework]]：说明 AI coding framework 的约束层可以扩展到视觉身份、组件 token 和设计验收。
- `支持` -> [[AI 工具化知识工作流]]：把设计判断资产化，并提供 lint、diff、export 等可复用工具动作。

## 回链

- 对应来源包主文件：[raw/repos/2026-07-14-github-google-labs-code-design-md/README.md](../../raw/repos/2026-07-14-github-google-labs-code-design-md/README.md)
