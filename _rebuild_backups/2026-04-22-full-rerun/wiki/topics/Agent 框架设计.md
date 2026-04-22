---
type: topic
status: active
tags:
  - Agent
  - Framework
  - GenericAgent
related_topics:
  - AI coding framework
related_concepts:
  - 自进化 Agent
source_pages:
  - GitHub - GenericAgent
  - Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent
updated: 2026-04-15
---

# Agent 框架设计

## 问题定义

这一页想回答：在当前这批来源里，一个 Agent 框架被如何定义，它最关键的设计抓手是什么。

## 当前结论

目前 GenericAgent 这组来源更支持一种“少工具、重沉淀、偏浏览器执行面”的设计路线。仓库 README 负责定义框架边界，社区帖子则负责放大它的传播标签。现阶段最稳的核心概念是“自进化 Agent”。

## 主要脉络

- [[GitHub - GenericAgent]] 是当前库里对该框架最稳的主说明来源，明确给出少工具、分层记忆、任务后沉淀 skill / SOP 等设计主张。
- [[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]] 负责展示项目在社区里是如何被包装和传播的。
- [[自进化 Agent]] 是这一组来源中最值得单独抽出的概念，因为它指向了“经验如何长期积累”的设计问题。
- 这组来源目前还不足以支持“显著优于同类工具”的强结论，更适合作为框架设计样本。

## 代表性来源

- [[GitHub - GenericAgent]]
- [[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]]

## 还不清楚的地方

- 浏览器能力、精度、token 优势等主张还缺独立 benchmark。
- `分层记忆`、`原子工具 Agent`、`SOP 固化` 这些二级概念还没正式落页。
- 目前仍难把“项目宣传口径”和“已验证能力”完全分开。

## 后续可追的问题

- 补 `分层记忆`、`原子工具 Agent`、`SOP 固化` 等概念页。
- 继续收集 GenericAgent 的独立验证材料，而不是只依赖 README 和论坛帖。
- 后面如果再有更多 Agent 框架样本，可以把这一页扩成更宽的比较主题。

## 相关概念

- [[自进化 Agent]]

## 相关主题

- [[AI coding framework]]
