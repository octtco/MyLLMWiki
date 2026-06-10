---
type: topic
status: active
tags:
  - AI Coding
  - Framework
related_topics:
  - Agent 框架设计
  - 代码库图谱化理解
  - AI 工具化知识工作流
  - 提示词设计
related_concepts:
  - Spec
  - Skill
source_pages:
  - GitHub - system-prompts-and-models-of-ai-tools
  - GitHub - claudesdk-skill
  - GitHub - Google Skills
  - GitHub - Trellis
  - Trellis Doc - 中文文档
  - GitHub - grill-me
  - Linux.do - 大道至简的胜利，一个神级 skill 推荐
  - Linux.do - Trellis + grill-me 组合用起来很爽
  - GitHub - MetaGPT
  - GitHub - awesome-ai-dev-prompts
  - GitHub - awesome-ai-software-development-agents
  - Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践
  - OpenAI - Work with Codex from anywhere
  - Google Blog - Gemini Intelligence brings proactive AI to Android
  - Kimi - WebBridge 功能页
  - GitHub - anthropic-cookbook
  - GitHub - awesome-chatgpt-prompts
  - GitHub - Bytebot
  - GitHub - Understand Anything
  - GitHub - CodeGraph
  - GitHub - andrej-karpathy-skills
  - GitHub - knowledge-work-plugins
  - GitHub - Multica
  - The Prompting Book
  - GitHub - Impeccable
  - GitHub - Compound Engineering
  - GitHub - revfactory Harness
  - GitHub - ECC
  - GitHub - Aegis
  - GitHub - gstack
  - GitHub - PraisonAI
  - GitHub - goose
updated: 2026-06-09
---

# AI coding framework

## 这页真正想回答什么

这页想回答的是：在当前这批来源里，什么样的东西才配叫作 AI coding framework，它和单个规则文件、一次性 prompt、零散脚本到底差在哪里。

## 为什么这个问题很容易讲散

如果只看表面，大家很容易把框架理解成“工具接入很多”“命令很多”或者“目录很多”。但这些都只是外观。真正会把问题讲散的，是没先分清一套框架到底在稳定什么。

## 当前最稳的主线

当前最稳的一条线来自 [[GitHub - Trellis]]、[[Trellis Doc - 中文文档]] 及其配套动机帖：所谓框架，不是把所有内容塞进一个文件里，而是把稳定约束层 [[Spec]]、按需调用的能力层 [[Skill]]、任务层和连续记忆一起组织成可复用工作流。

一旦接受这一点，很多表面分歧就会收束起来。`Spec` 不再是“比 skill 更重要”还是“该被 skill 取代”的问题，而是负责把项目里不该在每次新任务里重讲一遍的东西稳定下来；`Skill` 则负责把任务型能力、特殊工作流和输出纪律以可调用形式留下来。两者不是一套东西，也不是二选一。

## 这条主线是怎样往下走的

先有 [[GitHub - Trellis]] 给出结构定义：`.trellis/spec/`、`.trellis/tasks/`、`.trellis/workspace/` 这些层次本身就在说明，框架关心的是“怎样把规范、任务与连续性放进同一工作面”。

接着，[[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]] 又补了这套结构为什么会被需要：如果项目规范总得反复重讲，或者 skill 总是临场才想起来用，那所谓框架就还没真的站稳。

所以当前更稳的结论不是“Trellis 很强”，而是：在这组来源里，框架的关键价值是让约束、能力、任务和连续性不再各自飘着。

新补进来的 [[GitHub - grill-me]] 和两篇 Linux.do 使用帖，把这条主线往前推了一步：框架接住任务之前，需求本身也要先被问清楚。也就是说，稳定执行不只靠执行时的 task / spec / check，还要靠进入执行前的共享理解。这里更像 [[先追问到共享理解，再进入任务执行]]：先把 plan 或 design 的关键决策分支问到能共同指认，再让 Trellis 这类框架承接后续任务化执行。

再往横向看，[[GitHub - MetaGPT]]、[[GitHub - awesome-ai-dev-prompts]] 和 [[GitHub - awesome-ai-software-development-agents]] 让这页可以多一层边界感：Trellis 这类是框架，`awesome-ai-dev-prompts` 更像 prompt / role prompt 素材库，`awesome-ai-software-development-agents` 更像生态导航表。三者都和 AI coding 有关，但不能混成同一种东西。

这一轮外部核实又把这条线往外推了一点：所谓 AI coding framework，已经不只是“组织代码生成”的壳子，也开始变成“组织环境操作”的壳子。[[OpenAI - Work with Codex from anywhere]] 说明，至少在产品方向上，框架已经在接“远程派活、持续执行、查看进度、调用工具”这类系统级任务；它不再只是一段 prompt 加一个补全框。

[[Google Blog - Gemini Intelligence brings proactive AI to Android]] 则把另一种路线补了进来：agent 不一定待在 IDE 里，也可以直接嵌在操作系统和应用流里，负责跨 App 的多步执行。但当前更稳的写法仍然是“在用户控制下的上下文式执行”，还不适合直接写成“AI 已经会自主替你做完一切”。

[[Kimi - WebBridge 功能页]] 又提醒了另一个边界：不是所有“会点网页、会读页面”的东西都该叫完整框架。WebBridge 更像给现成模型接一座浏览器操作桥，让 Codex、Claude Code、Cursor、Kimi Code 这类执行体能看见页面、点击、填写、抽取内容。它很重要，但更像基础设施，不等于已经自己构成一套 AI coding framework。

这样一来，这页现在可以多保守收一层：框架的差别，已经不只体现在 `spec / skill / task / memory` 怎么组织，也体现在它能不能把电脑、浏览器、App 这些环境操作纳入同一工作面，而且还能把这些操作接回连续任务和可复用约束。

这次补入的一组 GitHub 仓库又把框架边界分得更细。[[GitHub - andrej-karpathy-skills]] 说明，单个规则文件可以约束 coding agent 的坏习惯，但它仍只是轻量纪律层；[[GitHub - Multica]] 则把 coding agents 放进任务分派、进度跟踪和技能沉淀的管理面，更接近 managed agents platform。

与此同时，[[GitHub - Understand Anything]] 和 [[GitHub - CodeGraph]] 把“框架需要怎样获得上下文”提到了前面。它们不是执行框架本身，而是给 Claude Code、Codex、Cursor 这类工具提供代码库图谱或本地预索引。这个方向现在单独放到 [[代码库图谱化理解]]，避免把索引层和执行层混成一件事。

最后，[[GitHub - anthropic-cookbook]]、[[GitHub - awesome-chatgpt-prompts]]、[[The Prompting Book]] 和 [[GitHub - knowledge-work-plugins]] 让框架外侧的素材层更清楚：cookbook 是官方配方，prompt 库是素材池，提示词设计把素材拆成角色、任务、格式、示例、上下文和链式流程，plugin 是角色 / 团队工作流打包。它们都能补框架生态，但只有当它们接回任务、验证和上下文供给时，才真正进入框架层。

这次补入的 [[GitHub - Impeccable]]、[[GitHub - Compound Engineering]] 和 [[GitHub - revfactory Harness]] 又把 skill / plugin 的边界推细了一层。Impeccable 把设计判断、前端反模式和视觉验收放进 AI coding 的可调用能力里；Compound Engineering 把 strategy、brainstorm、plan、work、review、compound note 做成工程闭环；revfactory Harness 则不是直接执行某个任务，而是尝试由领域描述生成 agent team 和 skills。它们共同说明：AI coding framework 已经不只是在“写代码”，也在扩展到设计纪律、工程组织和框架生成框架。

[[GitHub - ECC]] 再补了一层 cross-harness 视角：同一套 agentic work 不一定只绑定一个运行器，而可能把 skills、hooks、rules、memory 和 security 扩展成跨 Codex、Claude Code、Cursor、OpenCode 等环境的工作层。它让这页的边界更清楚：框架还包括“能力如何在不同 harness 之间迁移和治理”。

[[GitHub - Aegis]] 则把框架的重心压到工作纪律：先读 baseline、先明确架构边界、完成前要有新鲜证据、bug 修复要说明 repair 与 retirement。它不是 runtime，也不是最终完成判定器，更像给 AI coding agent 加一层可移植的方法包。

[[GitHub - gstack]] 又把这条线推到“虚拟工程团队”这一侧。它不是只提供一条 prompt 或一个审查命令，而是把 CEO、设计、工程管理、代码审查、QA、安全、发布、文档、retro、browser、spec 和 learn 这些角色 / 工具排进 `Think -> Plan -> Build -> Review -> Test -> Ship -> Reflect` 的顺序流程里。当前更稳的理解是：gstack 是一个角色化 skill stack 样本，说明 AI coding framework 可以把任务进入、计划复核、实现、验收和发布都纳入同一套可调用工作面。

[[GitHub - PraisonAI]] 和 [[GitHub - goose]] 又把框架边界往“可运行 host / workforce”方向推。PraisonAI 更像 agent workforce / workflow automation 平台，goose 更像本地桌面、CLI 和 API 形态的 agent host。它们都能服务 coding，但当前更稳的写法是：AI coding framework 正在和通用 agent host、MCP extension、workflow automation 平台靠近，而不是只剩 IDE 里的代码补全。

[[GitHub - Google Skills]] 和 [[GitHub - claudesdk-skill]] 又补了 skill 生态的两侧：前者是平台方把 Google 产品和技术能力整理成 Agent Skills，后者是个人实验项目把 Claude Agent SDK 文档、skill 和 webapp scaffold 串起来。它们共同说明，AI coding framework 的能力层正在从“项目内 prompt / rule”扩展到“平台 skill collection”和“SDK 理解型 skill”。

[[GitHub - system-prompts-and-models-of-ai-tools]] 从另一个角度提醒：coding agent 和 AI 工具的 system prompt / internal tools 会塑造框架行为，但泄露集合不能被当成官方接口或稳定设计文档。对框架研究更有用的是它暴露出的安全治理问题，而不是逐条复刻其中内容。

## 当前边界

- 这页现在已经补进 `grill-me + Trellis`、MetaGPT、两个 awesome 仓库这些横向样本，但仍不适合过早写成行业通论。
- `best harness`、`没有学习成本` 这类句子仍属于项目方口径。
- `grill-me > brainstorming > plan` 这类排序仍属于社区体验，不适合写成稳定结论。
- prompt 库和 awesome list 只适合当素材层或样本池，不等于已经验证过的框架方法。
- 提示词设计可以提供框架的基础材料，但单条 prompt 仍不能替代任务管理、上下文供给、工具调用和验收。
- Codex、Gemini 这类官方页当前更适合支持“系统级操作代理正在进入框架视野”这层判断，不适合直接外推成统一范式。
- WebBridge 更像浏览器控制桥，不该直接写成“会复刻网页的完整 agent 框架”。
- 单文件规则、prompt 库、cookbook、plugin、代码图谱和 managed agents platform 都只是框架生态的不同层，不应因为都服务 coding agent 就混成同一种东西。
- Impeccable、Compound Engineering 和 revfactory Harness 当前只按 README 与 GitHub 元数据整理，未验证安装体验、跨 harness 兼容性或真实项目效果。
- ECC 当前只按 README 与 GitHub 元数据整理，未验证安装叠加风险、hooks 行为、security scanning 和跨 harness 迁移成本。
- Aegis 当前只按 README 与 GitHub 元数据整理，未验证多 host 安装、activation mode、TDD routing 或 doctor 检查。
- gstack 当前只按 README 与 GitHub API 整理；生产力倍数、多 host 覆盖、team mode、browser / iOS / deploy / security 工具链都需要隔离测试后再推荐。
- PraisonAI 和 goose 当前只按 README 与 GitHub API 整理，未验证真实安装、provider 兼容、MCP 扩展、文件权限、shell 权限或长期任务表现。
- 当前更适合把这页当成“工作定义页”，不是横向优劣排行榜。

- Google Skills 和 claudesdk-skill 当前只按 README 与 GitHub API 整理，未验证具体 skill、认证、SDK 文档理解或端到端 webapp 生成。

## 代表性来源

- [[GitHub - system-prompts-and-models-of-ai-tools]]
- [[GitHub - claudesdk-skill]]
- [[GitHub - Google Skills]]
- [[GitHub - Trellis]]
- [[Trellis Doc - 中文文档]]
- [[GitHub - grill-me]]
- [[Linux.do - 大道至简的胜利，一个神级 skill 推荐]]
- [[Linux.do - Trellis + grill-me 组合用起来很爽]]
- [[GitHub - MetaGPT]]
- [[GitHub - awesome-ai-dev-prompts]]
- [[GitHub - awesome-ai-software-development-agents]]
- [[Linux.do - 经过 8 个月 Claude Code 高强度实战，我们决定开源内部的最佳实践]]
- [[OpenAI - Work with Codex from anywhere]]
- [[Google Blog - Gemini Intelligence brings proactive AI to Android]]
- [[Kimi - WebBridge 功能页]]
- [[GitHub - anthropic-cookbook]]
- [[GitHub - awesome-chatgpt-prompts]]
- [[GitHub - Bytebot]]
- [[GitHub - Understand Anything]]
- [[GitHub - CodeGraph]]
- [[GitHub - andrej-karpathy-skills]]
- [[GitHub - knowledge-work-plugins]]
- [[GitHub - Multica]]
- [[The Prompting Book]]
- [[GitHub - Impeccable]]
- [[GitHub - Compound Engineering]]
- [[GitHub - revfactory Harness]]
- [[GitHub - ECC]]
- [[GitHub - Aegis]]
- [[GitHub - gstack]]
- [[GitHub - PraisonAI]]
- [[GitHub - goose]]

## 相关概念

- [[Spec]]
- [[Skill]]

## 相关方法

- [[先追问到共享理解，再进入任务执行]]

## 相关主题

- [[Agent 框架设计]]
- [[代码库图谱化理解]]
- [[AI 工具化知识工作流]]
- [[提示词设计]]
