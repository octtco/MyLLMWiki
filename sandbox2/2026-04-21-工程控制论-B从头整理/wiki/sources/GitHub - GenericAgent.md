---
type: source
status: active
source_path: raw/repos/2026-04-14-github-lsdefine-genericagent/genericagent.md
source_type: repo_readme
source_url: https://github.com/lsdefine/GenericAgent
source_bundle: raw/repos/2026-04-14-github-lsdefine-genericagent
title: GenericAgent
authors:
  - lsdefine
year: 2026
created_at: 2026-04-14
updated_at: 2026-04-14
temporal_status: evolving
confidence: medium
claim_status: mixed
tags:
  - GenericAgent
  - Agent
  - Self-Evolving Agent
  - 分层记忆
  - 原子工具
  - Browser Agent
related_concepts:
  - 自进化 Agent
  - 分层记忆
  - 原子工具 Agent
  - SOP 固化
related_topics:
  - Agent 框架设计
---

# GenericAgent

## 一句话总结

GenericAgent 是一个主打“少工具、低 token、任务后自动沉淀为 skill”的通用 Agent 框架，README 重点强调极简执行面、分层记忆和自进化工作流。

## 摘要

- 这是项目仓库自己的主说明页，属于一手来源，能代表项目方对自身设计的定义。
- README 把项目定位成一个通用智能体框架，强调“少而准”的工具设计，而不是堆很多内置工具。
- 项目核心卖点包括：约 3K 行核心代码、9 个原子工具、四层分级记忆、任务后自动蒸馏为 skill。
- README 还强调浏览器执行面，认为结构化浏览器提取能显著降低 token 开销。
- 项目提供了安装与运行说明，也列出浏览器桥接、SOP 文件、记忆目录等配套资源。
- README 内带有和 Claude Code、OpenClaw 的对比口径，但这些对比首先应视为项目自述，不等于独立评测结论。

## 关键点

- 这份来源最重要的价值，是给出了 GenericAgent 的**自我定义**和**设计边界**。
- 项目不是把“工具多”当优势，而是把“原子工具少 + 调用更稳 + 记忆分层”当核心路线。
- “任务完成后沉淀为 skill / SOP” 是它区别于普通一次性 Agent 的关键叙事。
- 浏览器能力在 README 里被放得很重，说明 web 环境执行可能是这个项目的主战场之一。

## 证据或原文线索

- README 明确把项目叫作 `Self-Evolving Agentic Framework`。
- README 直接列出“约 3K 行核心代码”“9 个原子工具”“四层分级记忆”等主张。
- README 有安装步骤和运行方式，说明这不是纯概念稿，而是可运行项目。
- README 提到任务完成后会提炼成 skill，并给出 memory / SOP 相关路径。
- README 带有对 Claude Code、OpenClaw 的比较内容，但比较结果仍属于项目方口径。

## 可直接回证的能力或主张

- `约 3K 行核心代码`、`9 个原子工具`、`四层分级记忆` 这些都属于 README 直接写出的产品定义。
- `任务完成后沉淀为 skill / SOP`、`浏览器执行面`、`多模型兼容` 也都能在 README 的结构说明里找到对应表述。
- `自进化 Agent` 这条路线至少在项目命名和 README 叙事层面是明确成立的。

## 更偏项目方自述或待验证的判断

- 与 Claude Code、OpenClaw 的 token 对比和效果对比仍然主要是项目方口径。
- `Self-Bootstrap Proof` 这类“仓库全部由 Agent 自主完成”的说法，目前也还是 README 自述，不是独立验证结果。
- 浏览器能力和整体效率“显著优于”其他工具，这类判断需要独立 benchmark 才能沉淀成稳结论。

## 我的判断

- 这是一篇应该优先保留的主来源页，后续无论建概念页还是主题页，都应该先回链到这里。
- 目前可以相对稳地记的是：它怎么设计自己、怎么组织执行面、怎么组织记忆与 skill。
- 暂时不能直接当成已证实事实的，是 README 中所有“显著优于某某”“token 大幅更省”“效果更强”这类对比结论。
- 如果后面要继续整理，最值得补的不是马上扩写主题页，而是补仓库快照或关键文件摘录，增强可追溯性。

## 相关概念

- [[自进化 Agent]]
- 分层记忆
- 原子工具 Agent
- SOP 固化

## 相关主题

- [[Agent 框架设计]]

## 关系

- `定义` -> [[自进化 Agent]]：这页是项目方主说明，当前库里对该概念的定义支撑最稳。
- `支持` -> [[Agent 框架设计]]：README 直接给出框架定位、能力边界和执行组织方式。
- `主说明` -> [[Linux.do - GenericAgent 仅仅~3K 行代码 Self-Evolving Agent]]：本页偏项目自述，论坛帖更像传播层和补充口径。

## 回链

- 对应原始文件：[raw/repos/2026-04-14-github-lsdefine-genericagent/genericagent.md](../../raw/repos/2026-04-14-github-lsdefine-genericagent/genericagent.md)
- 对应外部来源：[GitHub - lsdefine/GenericAgent](https://github.com/lsdefine/GenericAgent)
