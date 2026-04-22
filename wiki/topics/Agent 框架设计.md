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
updated: 2026-04-22
---

# Agent 框架设计

## 这页真正想回答什么

这页想回答的是：在当前这组来源里，一个 agent 框架最关键的设计抓手到底是什么。

## 为什么这个问题很容易讲散

大家谈 agent 框架时，很容易把注意力全放在工具个数、跑分、浏览器能力或者 token 消耗上。它们当然重要，但如果只停在这里，问题会变成一堆并列参数，而不是一套设计判断。

## 当前最稳的主线

当前 GenericAgent 这组来源更支持这样一条线：agent 框架的关键不只是“会不会做事”，而是它有没有办法把做过的事沉淀下来，让下次不必再从零开始。

这也是为什么 [[自进化 Agent]] 会在这里变成最核心的概念。只要任务经验不能稳定落成 [[Skill]] 或 SOP，框架再能跑，也更像一次次临场发挥；一旦能沉淀，框架才开始拥有长期能力积累这层意义。

## 这条主线是怎样往下走的

[[GitHub - GenericAgent]] 先给出了比较清楚的结构定义：分层记忆、最小工具集和任务后固化技能，是它理解 agent 的三个核心部件。

[[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]] 则把这件事推成了传播标签。帖子把“9 个工具”“3K 行代码”“自动蒸馏 SOP”放得很响，同时评论区也立刻把问题顶了回来：这些能力到底怎么验证。

所以当前更稳的结论不是“它显著强于别家”，而是：这组来源最值得保留的设计问题，是经验如何沉淀，而不是工具怎么继续堆。

## 当前边界

- 这页目前主要由项目 README 和论坛推广帖支撑，外部验证材料还不够。
- 浏览器能力、精度、token 优势等更强说法仍应停留在待验证状态。
- 当前这页更适合当框架样本页，不适合直接扩成横向结论页。

## 代表性来源

- [[GitHub - GenericAgent]]
- [[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]]

## 相关概念

- [[自进化 Agent]]
- [[Skill]]

## 相关主题

- [[AI coding framework]]
