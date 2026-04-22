---
type: source
status: active
source_path: raw/repos/2026-04-14-github-mindfold-ai-trellis/trellis.md
source_type: repo
source_url: https://github.com/mindfold-ai/Trellis
source_bundle: raw/repos/2026-04-14-github-mindfold-ai-trellis
title: GitHub - Trellis
authors:
  - mindfold-ai
created_at: 2026-04-22
updated_at: 2026-04-22
tags:
  - AI Coding
  - Framework
  - Spec
  - Task
  - Memory
related_concepts:
  - Spec
  - Skill
related_topics:
  - AI coding framework
related_relations: []
---

# GitHub - Trellis

## 一句话总结

这份 README 把 Trellis 定义成一种多平台 AI coding framework：核心不是单个 prompt，而是把 `spec`、`tasks`、`workspace memory` 和平台接线一起组织成可复用工作流。

## 摘要

- 项目把 `.trellis/` 设成核心目录，里面同时放规范层、任务层、工作区记忆和工作流脚本。
- README 反复强调 `spec`、`task-centered workflow`、`project memory` 和 `parallel agent execution` 这几个抓手。
- 这个来源最稳的价值不在“最好”这类宣传词，而在它给出了一个结构化 AI coding framework 的清晰样板。

## 证据或原文线索

- `Why Trellis?` 段落把 `Auto-injected specs`、`Task-centered workflow`、`Project memory`、`Parallel agent execution` 并列列出。
- `How It Works` 直接给出 `.trellis/` 目录结构：`spec/`、`tasks/`、`workspace/`、`workflow.md`、`scripts/`。
- FAQ 里明确把 Trellis 和单独的 `CLAUDE.md`、`AGENTS.md`、`.cursorrules` 区分开，说明它主张的是更高层的工作流组织。

## 我的判断

- 当前库里，这份来源足够支撑一个较稳的 [[AI coding framework]] 来源页。
- 它也足够支撑 [[Spec]] 和 [[Skill]] 作为两个原子概念进入知识网络。
- 但 `The best agent harness` 这类句子属于项目方口径，不适合直接写成稳定结论。

## 相关概念

- [[Spec]]
- [[Skill]]

## 相关主题

- [[AI coding framework]]

## 关系

- `定义` -> [[Spec]]：README 明确把规范层放进工作流核心结构里。
- `支持` -> [[Skill]]：README 虽然没有把 skill 当唯一核心，但明确承认按需扩展能力层的存在。
- `支持` -> [[AI coding framework]]：这份来源给出了当前库里最完整的一种框架级定义。

## 回链

- 对应来源包主文件：[raw/repos/2026-04-14-github-mindfold-ai-trellis/trellis.md](../../raw/repos/2026-04-14-github-mindfold-ai-trellis/trellis.md)
