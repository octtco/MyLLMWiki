---
type: topic
status: active
tags:
  - Agent
  - Framework
related_topics:
  - AI coding framework
related_concepts:
  - 自进化 Agent
  - Skill
source_pages:
  - GitHub - GenericAgent
  - Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent
  - GitHub - MetaGPT
  - GitHub - awesome-ai-software-development-agents
updated: 2026-05-15
---

# Agent 框架设计

## 这页真正想回答什么

这页想回答的是：在当前这组来源里，一个 agent 框架最关键的设计抓手到底是什么。

## 为什么这个问题很容易讲散

大家谈 agent 框架时，很容易把注意力全放在工具个数、跑分、浏览器能力或者 token 消耗上。它们当然重要，但如果只停在这里，问题会变成一堆并列参数，而不是一套设计判断。

## 当前最稳的主线

当前 GenericAgent 这组来源更支持这样一条线：agent 框架的关键不只是“会不会做事”，而是它有没有办法把做过的事沉淀下来，让下次不必再从零开始。

这也是为什么 [[自进化 Agent]] 会在这里变成最核心的概念。只要任务经验不能稳定落成 [[Skill]] 或 SOP，框架再能跑，也更像一次次临场发挥；一旦能沉淀，框架才开始拥有长期能力积累这层意义。

[[GitHub - MetaGPT]] 则补了另一条路线：不是先问“单个 agent 怎样进化”，而是先把软件开发看成一家公司式的多角色协作。它用 SOP 和角色团队组织产品、架构、工程等环节，说明 agent 框架也可以从“一个聪明执行者”转向“多角色流程编排”。

## 这条主线是怎样往下走的

[[GitHub - GenericAgent]] 先给出了比较清楚的结构定义：分层记忆、最小工具集和任务后固化技能，是它理解 agent 的三个核心部件。

[[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]] 则把这件事推成了传播标签。帖子把“9 个工具”“3K 行代码”“自动蒸馏 SOP”放得很响，同时评论区也立刻把问题顶了回来：这些能力到底怎么验证。

接着 [[GitHub - MetaGPT]] 把 SOP 放到团队流程层，而不是只放到任务后经验沉淀层。这样一来，当前这页可以保守地区分两种抓手：一种是任务结束后怎样沉淀经验，另一种是任务开始时怎样分配角色和流程。

所以当前更稳的结论不是“谁显著强于别家”，而是：agent 框架设计至少有两条值得继续观察的路线，经验沉淀路线和多角色 SOP 编排路线。[[GitHub - awesome-ai-software-development-agents]] 这类导航表先用来扩样本池，不直接当质量证明。

## 当前边界

- 这页目前主要由项目 README、论坛推广帖和 awesome list 入口支撑，外部验证材料还不够。
- 浏览器能力、精度、token 优势等更强说法仍应停留在待验证状态。
- awesome list 只能证明生态里有这些入口，不能证明列表内项目都稳定好用。
- 当前这页更适合当框架样本页，不适合直接扩成横向结论页。

## 代表性来源

- [[GitHub - GenericAgent]]
- [[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]]
- [[GitHub - MetaGPT]]
- [[GitHub - awesome-ai-software-development-agents]]

## 相关概念

- [[自进化 Agent]]
- [[Skill]]

## 相关主题

- [[AI coding framework]]
