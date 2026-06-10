---
type: source
status: active
source_path: raw/repos/2026-05-28-github-simstudioai-sim/sim.md
source_type: repo
source_url: https://github.com/simstudioai/sim
source_bundle: raw/repos/2026-05-28-github-simstudioai-sim
title: GitHub - Sim
authors:
  - simstudioai
created_at: 2026-05-28
updated_at: 2026-05-28
tags:
  - Agent
  - Workflow
  - Automation
related_methods: []
related_concepts: []
related_topics:
  - Agent 框架设计
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - Sim

## 一句话总结

Sim 是一个面向 AI agent workflow 的开源平台样本，README 把它定位为“构建、部署和编排 AI agents / agentic workforce”的可视化工作台。

## 当前范围

本页只整理 GitHub README 和仓库元数据，不安装自托管版本，不验证 1,000+ integrations、Copilot 和 vector database 功能。

## 摘要

- README 把 Sim 描述为 open-source platform，用来构建 AI agents 并运行 agentic workforce。
- 它强调可视化 canvas：连接 agents、tools 和 blocks 后运行 workflow。
- README 提到 Copilot 可以用自然语言生成节点、修复错误和迭代 flow。
- 它支持文档上传到 vector store，让 agent 基于特定内容回答问题。
- 自托管路径包括 `npx simstudio`、Docker Compose 和手动安装；技术栈包括 Next.js、Bun、PostgreSQL/pgvector、ReactFlow、Trigger.dev、E2B 等。

## 证据或原文线索

- GitHub API 抓取时显示 Apache-2.0 license，stars 约 28.6k，仓库未归档。
- README heading 包括 `Build Workflows with Ease`、`Supercharge with Copilot`、`Integrate Vector Databases`、`Quickstart`、`Tech Stack`。
- 仓库 homepage 指向 `https://www.sim.ai`。

## 当前可支持的判断

- 当前来源支持：Sim 代表一类把 agent 编排放进可视化 workflow builder 的平台路线。
- 当前可保守迁出：agent 工具不一定只以聊天框或 CLI 形式存在，也可以落成带节点、工具、知识库和部署形态的工作流画布。

## 当前边界

- README 里的集成数量、Copilot 效果和自托管体验没有实测，不能写成已验证结论。
- 这页不评价 Sim 与 Dify、n8n、LangGraph Studio 等平台的优劣。

## 相关主题

- [[Agent 框架设计]]
- [[AI 工具化知识工作流]]

## 关系

- `支持` -> [[Agent 框架设计]]：提供可视化 agent workflow 编排样本。
- `补充` -> [[AI 工具化知识工作流]]：把 AI 工具化工作流从 prompt / plugin / 终端扩到 agent workflow builder。

## 回链

- 对应来源包主文件：[raw/repos/2026-05-28-github-simstudioai-sim/sim.md](../../raw/repos/2026-05-28-github-simstudioai-sim/sim.md)

