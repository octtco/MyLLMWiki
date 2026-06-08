---
type: source
status: review
source_path: raw/repos/2026-06-05-github-frankhuy-fishkeeper/fishkeeper.md
source_type: repo
source_url: https://github.com/FrankHuy/fishkeeper
source_bundle: raw/repos/2026-06-05-github-frankhuy-fishkeeper
title: GitHub - fishkeeper
authors:
  - FrankHuy
created_at: 2026-06-05
updated_at: 2026-06-05
tags:
  - Agent
  - Skill
  - Ecommerce
  - Review
related_methods: []
related_concepts:
  - Skill
related_topics:
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - fishkeeper

## 一句话总结

fishkeeper 是一个面向闲鱼 / 闲管家开放平台的 Hermes Agent Skill，用 Python 客户端和编排器把商品管理、订单处理、库存同步等店铺运营动作接入 agent 工作流。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未安装 skill，未配置闲管家 API 凭据，未调用真实店铺、商品、订单、发货或 Webhook 接口。

## 摘要

- README 把 `fishkeeper` 解释为“闲管家”的品牌名，skill 名 `goofish` 对应 Goofish Open Platform 的 API 标识。
- 功能覆盖商品全生命周期管理、订单查询 / 发货 / 改价 / 卡密查询、类目 / 属性 / 规格查询、库存快照、批量上架、批量发货和 MD5 签名认证。
- 项目结构以 `skills/goofish/` 为核心，包含 `SKILL.md`、配置模板、`signer.py`、`client.py`、`orchestrator.py`、API reference 和 multi-agent patterns。
- README 提供 Hermes Agent、Claude Code、Codex CLI、Cursor / Windsurf、MCP Server 和自定义 Agent 框架的集成方式。
- GitHub API 抓取时显示 Python 仓库、MIT license、stars 约 4、未归档；仓库创建于 2026-06-03。

## 当前可支持的判断

- 当前来源支持：fishkeeper 是一个面向闲鱼店铺运营的垂直业务 Skill，而不是通用 agent 框架。
- 当前可保守迁出：它补充 [[AI 工具化知识工作流]] 中“业务 API + agent skill + 编排脚本”这一类资产形态，说明知识工作流可以下沉到电商运营动作。
- 当前只适合把它保存为电商 / 店铺运营自动化的早期样本，不适合直接写成可生产推荐。

## 当前边界

- README 未能替代闲管家官方 API 文档、平台规则、店铺授权和数据合规要求。
- 商品上下架、改价、发货、卡密查询和库存同步都可能直接影响真实交易，后续测试必须使用沙箱、测试店铺或只读模式。
- API 凭据、签名、Webhook 和订单数据都涉及安全边界；当前不把安装片段升级成生产部署教程。
- 仓库很新且 stars 很少，当前只按来源入口保存，不判断维护稳定性。

## 相关主题

- [[AI 工具化知识工作流]]

## 关系

- `补充` -> [[AI 工具化知识工作流]]：提供垂直业务 API 被封装成 agent skill 和多 agent 编排脚本的样本。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-05-github-frankhuy-fishkeeper/fishkeeper.md](../../raw/repos/2026-06-05-github-frankhuy-fishkeeper/fishkeeper.md)
