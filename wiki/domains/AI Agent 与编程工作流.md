---
type: domain
status: review
tags:
  - AI Coding
  - Agent
  - Workflow
related_topics:
  - AI coding framework
  - Agent 框架设计
  - 代码库图谱化理解
  - Agent 记忆与知识图谱
  - 提示词设计
related_methods:
  - 先追问到共享理解，再进入任务执行
related_concepts:
  - Spec
  - Skill
  - 自进化 Agent
related_domains:
  - AI 工具化知识工作流
source_pages:
  - GitHub - Trellis
  - GitHub - MetaGPT
  - GitHub - gstack
  - GitHub - goose
  - GitHub - Google Skills
updated: 2026-06-09
---

# AI Agent 与编程工作流

## 这页覆盖什么长期问题域

这个领域入口覆盖的是：AI agent 如何进入软件开发工作流，并把需求澄清、任务拆解、代码理解、实现、评审、测试、发布和经验沉淀组织成可复用流程。

它不是编程工具列表，而是用来导航“AI coding 从一次性补全变成持续工程协作”这条主线。

## 当前关键主题

- [[AI coding framework]]：组织 spec、skill、task、memory 和环境操作的主入口。
- [[Agent 框架设计]]：多角色、workflow、runtime、memory 和 orchestration 的框架问题。
- [[代码库图谱化理解]]：agent 进入代码库之前怎样获得结构化上下文。
- [[Agent 记忆与知识图谱]]：长期任务里上下文如何保持、更新和召回。
- [[提示词设计]]：prompt 作为框架材料，而不是完整框架本身。

## 当前关键方法

- [[先追问到共享理解，再进入任务执行]]：在进入框架执行前，先把需求和设计分支问清楚。

## 当前关键概念

- [[Spec]]
- [[Skill]]
- [[自进化 Agent]]

## 主要来源

- [[GitHub - Trellis]]
- [[GitHub - MetaGPT]]
- [[GitHub - gstack]]
- [[GitHub - goose]]
- [[GitHub - Google Skills]]

## 当前缺口

- 很多来源只整理 README，缺少安装、真实任务和失败样本验证。
- 多 host、MCP、浏览器、桌面权限和长期记忆的安全边界还需要单独复核。
- 还缺少从真实项目端到端跑完的案例页。

## 后续可扩方向

- 从 `AI coding framework` 里继续筛代表性案例。
- 把“代码库上下文供给”和“执行框架”拆得更清楚。
- 对 gstack、goose、PraisonAI、ECC 等来源做隔离跑测后再更新状态。

## 相关领域

- [[AI 工具化知识工作流]]
