---
type: topic
status: review
tags:
  - Knowledge Work
  - AI Tool
  - Workflow
related_topics:
  - AI coding framework
  - Agent 框架设计
  - Agent 记忆与知识图谱
  - 提示词设计
related_methods: []
related_concepts:
  - Skill
  - 可观测性
related_relations: []
source_pages:
  - GitHub - anthropic-cookbook
  - GitHub - awesome-chatgpt-prompts
  - GitHub - knowledge-work-plugins
  - GitHub - Presenton
  - GitHub - FinceptTerminal
  - GitHub - AI Engineering from Scratch
  - The Prompting Book
  - GitHub - MarkItDown
  - GitHub - Sim
  - GitHub - Open Deep Research
  - GitHub - MindsDB
  - GitHub - Graphiti
  - GitHub - MoneyPrinterTurbo
  - GitHub - Supermemory
  - GitHub - Compound Engineering
  - GitHub - Production Agentic RAG Course
  - GitHub - fishkeeper
  - GitHub - Prompt Engineering Interactive Tutorial
  - GitHub - Vanna
  - GitHub - PraisonAI
  - GitHub - AIHawk
  - GitHub - MCP Toolbox for Databases
  - GitHub - open-notebook
updated: 2026-06-08
---

# AI 工具化知识工作流

## 这页到底在回答什么

这页想收住一个问题：AI 进入知识工作以后，什么时候只是聊天助手，什么时候开始变成可复用、可部署、可交付的工具化工作流。

## 为什么这个问题会让人反复做散

知识工作 AI 很容易被讲成“能写文案”“能做 PPT”“能查金融数据”“能生成 prompt”。这些说法都对，但如果不区分资产形态，就会把 prompt 库、API cookbook、插件市场、垂直终端和交付物生成器混成一类。

## 当前最稳的主线

当前这组来源支持的主线是：AI 知识工作流正在从一次性对话，分化成几种可复用资产。[[GitHub - awesome-chatgpt-prompts]] 代表 prompt 资产化，[[The Prompting Book]] 说明这些 prompt 资产怎样继续被拆成设计构件和工作流技巧，[[GitHub - anthropic-cookbook]] 代表 API 配方化，[[GitHub - knowledge-work-plugins]] 代表角色 / 团队流程插件化，[[GitHub - Presenton]] 和 [[GitHub - FinceptTerminal]] 则把输出和数据探索推向具体工作台。最近补入的 [[GitHub - MarkItDown]]、[[GitHub - Sim]]、[[GitHub - Open Deep Research]]、[[GitHub - MindsDB]]、[[GitHub - Graphiti]]、[[GitHub - MoneyPrinterTurbo]]、[[GitHub - Supermemory]]、[[GitHub - Compound Engineering]]、[[GitHub - Production Agentic RAG Course]]、[[GitHub - fishkeeper]]、[[GitHub - Vanna]]、[[GitHub - MCP Toolbox for Databases]]、[[GitHub - open-notebook]]、[[GitHub - PraisonAI]] 和 [[GitHub - AIHawk]] 又把入口扩到文档 ingest、agent workflow、deep research、企业 AI 平台、agent memory 基础设施、短视频生产流水线、工程协作闭环、生产级 RAG 学习链路、电商运营 API skill、数据库 MCP / Text-to-SQL、自托管研究工作台和求职流程自动化。

## 这条主线怎样一段一段展开

第一段是 prompt 资产化。prompt 库让“怎么问”可以被收藏、分享、自托管，[[The Prompting Book]] 则补了中间层：prompt 还需要被拆成角色、背景、任务、约束、格式、示例、迭代和上下文供给，才有机会从素材继续走向可复用工作流。

第二段是工程配方化。cookbook 把 API 能力变成可复制代码片段，让开发者能把能力接进自己的系统。

第三段是插件化。knowledge-work-plugins 把 skills、connectors、slash commands、sub-agents 放在一个插件边界里，说明团队知识工作可以被打包成可安装能力。

第四段是交付物和垂直终端。Presenton 把 presentation 生成做成应用和 API，FinceptTerminal 把金融数据、分析和探索放进专业终端。它们说明知识工作 AI 不一定停在聊天框，可能落成具体产物界面。

第五段是输入、研究和平台化。MarkItDown 先把复杂文件转成 Markdown，让材料进入 LLM 管线；Sim 把 agent 编排放进可视化 workflow builder；Open Deep Research 把研究任务拆成搜索、研究、压缩、报告和评估；MindsDB 则把 automation agent、semantic search、部署控制和企业数据场景合在一块。Graphiti 和 Supermemory 再补一层记忆基础设施：工作流如果要长期运行，还需要让上下文能随事实变化增量更新。MoneyPrinterTurbo 则代表内容生产端的流水线化，把脚本、配音、字幕、素材和视频输出组织起来。这样看，工具化知识工作流的关键不只是“模型能生成什么”，还包括材料怎样进来、任务怎样编排、结果怎样评估、上下文怎样保真，以及系统怎样部署在可控边界里。

第六段是工程协作本身的工具化。[[GitHub - Compound Engineering]] 把 strategy、brainstorm、plan、work、debug、review 和 compound note 组织成一组可安装 skills / agents，说明知识工作流不只服务外部交付物，也可以服务工程团队内部的计划、评审和经验沉淀。

第七段是 RAG 生产化。[[GitHub - Production Agentic RAG Course]] 把论文摄取、搜索、chunking、hybrid retrieval、RAG、监控、缓存和 agentic control 串成课程项目，说明知识工作流要稳定运行时，检索、可观测性和服务编排会和模型回答同等重要。

第八段是垂直业务 API skill 化。[[GitHub - fishkeeper]] 把闲鱼 / 闲管家开放平台的商品、订单、库存和发货动作封装成 Hermes skill、Python client 和多 agent 编排脚本。它提醒这页：工具化知识工作流不只发生在研究、内容和工程协作里，也会落到真实业务系统的 API 操作层；但这类工具一旦触达交易、库存和发货，就必须把授权、凭据、平台规则和可回滚性放在前面。

第九段是数据库和研究工作台。[[GitHub - Vanna]] 把自然语言、SQL、权限过滤、图表和摘要合成一个数据问答界面；[[GitHub - MCP Toolbox for Databases]] 则把数据库访问放进 MCP server 和 custom tools framework；[[GitHub - open-notebook]] 把多模态材料、检索、对话和播客生成收成自托管 Notebook LM 替代品。它们共同说明：知识工作流落地时，最难的往往不是“让模型回答”，而是把数据权限、资料摄取、检索、审计和用户界面一起管住。

第十段是自动化业务流程。[[GitHub - PraisonAI]] 把 agent workforce、flow builder 和 dashboard 放进多 agent 工作流；[[GitHub - AIHawk]] 则把求职投递流程自动化作为高风险样本。前者提醒 workflow automation 正在平台化，后者提醒一旦 AI 代替人和外部平台交互，就会碰到平台条款、身份真实性、反滥用和个人数据安全。

## 代表性来源

- [[GitHub - anthropic-cookbook]]
- [[GitHub - awesome-chatgpt-prompts]]
- [[GitHub - knowledge-work-plugins]]
- [[GitHub - Presenton]]
- [[GitHub - FinceptTerminal]]
- [[GitHub - AI Engineering from Scratch]]
- [[The Prompting Book]]
- [[GitHub - MarkItDown]]
- [[GitHub - Sim]]
- [[GitHub - Open Deep Research]]
- [[GitHub - MindsDB]]
- [[GitHub - Graphiti]]
- [[GitHub - MoneyPrinterTurbo]]
- [[GitHub - Supermemory]]
- [[GitHub - Compound Engineering]]
- [[GitHub - Production Agentic RAG Course]]
- [[GitHub - fishkeeper]]
- [[GitHub - Prompt Engineering Interactive Tutorial]]
- [[GitHub - Vanna]]
- [[GitHub - PraisonAI]]
- [[GitHub - AIHawk]]
- [[GitHub - MCP Toolbox for Databases]]
- [[GitHub - open-notebook]]

## 当前边界

- 这页只做工具形态整理，不评价每个工具质量。
- 金融终端来源不提供投资建议。
- Prompt 库和插件市场都需要后续抽样验证，不能只看 stars。
- MarkItDown、Sim、Open Deep Research、MindsDB、Graphiti、MoneyPrinterTurbo、Supermemory、Compound Engineering、Production Agentic RAG Course、fishkeeper、Vanna、PraisonAI、AIHawk、MCP Toolbox 和 open-notebook 当前都只按 README 入口整理，未做真实任务跑测。
- MoneyPrinterTurbo 这类内容生成工具还要单独复核素材版权、平台规则和批量生成边界。
- fishkeeper 这类电商运营 API skill 还要单独复核平台授权、店铺数据安全、订单操作风险和凭据管理边界。
- Vanna 和 MCP Toolbox 这类数据库工具必须先按只读、样例库、最小权限和审计日志复核。
- AIHawk 这类求职自动化工具涉及平台条款、招聘公平性、身份真实性和个人数据安全，当前不迁出操作步骤。

## 后续可追的问题

- 选一个真实知识工作任务，对比 prompt 库、cookbook、plugin、专用工具哪种形态最省力。
- 如果后续继续积累同类工具，可拆出“prompt 资产化”“插件化知识工作”两个概念候选。

## 关系

- `支持` <- [[GitHub - anthropic-cookbook]]：提供 API 配方化样本。
- `支持` <- [[GitHub - awesome-chatgpt-prompts]]：提供 prompt 资产化样本。
- `支持` <- [[The Prompting Book]]：提供提示词从构件到工作流的长书骨架。
- `支持` <- [[GitHub - knowledge-work-plugins]]：提供知识工作 plugin 市场样本。
- `支持` <- [[GitHub - Presenton]]：提供演示文稿生成工具样本。
- `支持` <- [[GitHub - FinceptTerminal]]：提供金融研究终端样本。
- `补充` <- [[GitHub - AI Engineering from Scratch]]：提供学习到交付的课程型知识工作样本。
- `支持` <- [[GitHub - MarkItDown]]：提供文档转 Markdown / LLM 输入整理样本。
- `支持` <- [[GitHub - Sim]]：提供可视化 agent workflow builder 样本。
- `支持` <- [[GitHub - Open Deep Research]]：提供 deep research agent 工作流样本。
- `支持` <- [[GitHub - MindsDB]]：提供企业 AI 平台和 semantic search 样本。
- `补充` <- [[GitHub - Graphiti]]：提供 temporal context graph / agent memory 基础设施样本。
- `支持` <- [[GitHub - MoneyPrinterTurbo]]：提供短视频自动化生成工具样本。
- `补充` <- [[GitHub - Supermemory]]：提供 AI memory / context API 和 MCP 样本。
- `补充` <- [[GitHub - Compound Engineering]]：提供工程协作闭环和经验沉淀 plugin 样本。
- `补充` <- [[GitHub - Production Agentic RAG Course]]：提供生产级 RAG / agentic RAG 课程项目样本。
- `补充` <- [[GitHub - fishkeeper]]：提供垂直业务 API 封装成 agent skill 和多 agent 编排脚本的样本。
- `补充` <- [[GitHub - Prompt Engineering Interactive Tutorial]]：提供官方交互式 prompt 教程样本。
- `支持` <- [[GitHub - Vanna]]：提供自然语言到 SQL / 数据洞察工具样本。
- `补充` <- [[GitHub - PraisonAI]]：提供 agent workforce / workflow automation 平台样本。
- `待验证` <- [[GitHub - AIHawk]]：提供求职自动化 agent 的高风险边界样本。
- `支持` <- [[GitHub - MCP Toolbox for Databases]]：提供数据库 MCP server 和 custom tools framework 样本。
- `支持` <- [[GitHub - open-notebook]]：提供自托管研究工作台 / Notebook LM 替代样本。

## 相关概念

- [[Skill]]
- [[可观测性]]
