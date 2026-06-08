---
type: source
status: review
source_path: raw/repos/2026-06-08-github-vanna-ai-vanna/vanna.md
source_type: repo
source_url: https://github.com/vanna-ai/vanna
source_bundle: raw/repos/2026-06-08-github-vanna-ai-vanna
title: GitHub - Vanna
authors:
  - vanna-ai
created_at: 2026-06-08
updated_at: 2026-06-08
tags:
  - Text-to-SQL
  - Database
  - Agent
  - Review
related_methods: []
related_concepts: []
related_topics:
  - AI 工具化知识工作流
related_cases: []
related_relations: []
---

# GitHub - Vanna

## 一句话总结

Vanna 是一个把自然语言问题转换为 SQL 和数据洞察的 Text-to-SQL 工具，README 强调 user-aware permissions、流式结果、图表、审计日志和 Web Component。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未连接真实数据库，未验证 SQL 生成准确性、权限过滤、审计日志或 Web Component。

## 摘要

- README 把 Vanna 2.0 定位为 Natural language -> SQL -> Answers。
- 功能口径包括 `<vanna-chat>` Web Component、流式表格 / 图表 / 摘要、row-level security、audit logs、rate limiting、FastAPI / Flask 集成和 observability。
- README 声称支持多种 LLM 和 PostgreSQL、MySQL、Snowflake、BigQuery、SQLite、Oracle、SQL Server、DuckDB、ClickHouse 等数据库。
- GitHub API 抓取时显示 Python 仓库，MIT license，stars 约 23577，但仓库当前 archived。

## 当前可支持的判断

- 当前来源支持：Vanna 是数据库问答和 Text-to-SQL 的工具化知识工作流样本。
- 当前可保守迁出：它补充 [[AI 工具化知识工作流]] 中“业务数据 -> 自然语言查询 -> SQL / 图表 / 摘要”的应用形态。

## 当前边界

- 仓库当前 archived，不能按活跃项目推荐。
- Text-to-SQL 直接触达数据库，后续测试必须先限制只读权限、样例库和查询配额。
- README 的 enterprise security、权限过滤和准确性口径需要真实数据库和权限模型复测。

## 相关主题

- [[AI 工具化知识工作流]]

## 回链

- 对应来源包主文件：[raw/repos/2026-06-08-github-vanna-ai-vanna/vanna.md](../../raw/repos/2026-06-08-github-vanna-ai-vanna/vanna.md)
