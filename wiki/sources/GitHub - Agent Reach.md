---
type: source
status: review
source_path: raw/repos/2026-06-09-github-panniantong-agent-reach/agent-reach.md
source_type: repo
source_url: https://github.com/Panniantong/Agent-Reach
source_bundle: raw/repos/2026-06-09-github-panniantong-agent-reach
title: GitHub - Agent Reach
authors:
  - Panniantong
created_at: 2026-06-09
updated_at: 2026-06-09
tags:
  - Agent
  - Research
  - Skill
  - Review
related_methods: []
related_concepts:
  - Skill
related_topics:
  - AI 工具化知识工作流
  - Agent 框架设计
related_cases: []
related_relations: []
---

# GitHub - Agent Reach

## 一句话总结

Agent Reach 是一个给 AI agent 接入多平台读取与搜索能力的 CLI / skill，覆盖 Twitter、Reddit、YouTube、GitHub、Bilibili、小红书等渠道。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未安装 CLI，未配置 cookie/token，未测试各平台搜索、读取、脚本提取或卸载流程。

## 摘要

- README 用中文说明“Give your AI agent eyes to see the entire internet”，并列出 Twitter、Reddit、YouTube、GitHub、Bilibili、小红书等平台。
- 设计理念强调每个渠道可插拔，并包含安全性、Cookie 安全建议、安装和卸载章节。
- GitHub API 抓取时显示 Python 仓库，MIT license，未归档。
- GitHub API 抓取时显示 Python 仓库，MIT license，stars 约 24370，仓库未归档。

## 当前可支持的判断

- 当前来源支持：Agent Reach 是 agent 外部信息源接入层样本。
- 它补充 [[AI 工具化知识工作流]]：公开平台信息采集可以从手工搜索变成 agent 可调用渠道。
- 它也补充 [[Agent 框架设计]]：agent 的“看见互联网”能力应被放进插件/skill 权限边界，而不是默认无限开放。

## 当前边界

- 多平台抓取涉及平台条款、登录态、cookie 安全、隐私和限流。
- 抖音 / 小红书脚本提取等可选实现需要额外审查，不迁出规避限制或绕授权步骤。
- 当前不把它写成 OSINT 教程，只作为 agent reach / channel connector 样本保存。

## 相关主题

- [[AI 工具化知识工作流]]
- [[Agent 框架设计]]

## 关系

- `补充` -> [[AI 工具化知识工作流]]：提供本来源在该主题下的主要样本。
- `轻量补充` -> [[Agent 框架设计]]：提供相邻问题的补充样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-09-github-panniantong-agent-reach/agent-reach.md](../../raw/repos/2026-06-09-github-panniantong-agent-reach/agent-reach.md)
