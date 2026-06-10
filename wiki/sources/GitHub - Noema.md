---
type: source
status: active
source_path: raw/repos/2026-06-09-github-happyfox001-noema/noema.md
source_type: repo
source_url: https://github.com/HappyFox001/Noema
source_bundle: raw/repos/2026-06-09-github-happyfox001-noema
title: GitHub - Noema
authors:
  - HappyFox001
created_at: 2026-06-09
updated_at: 2026-06-09
tags:
  - Agent
  - Voice Assistant
  - Desktop
  - Review
related_methods: []
related_concepts:
  - Skill
related_topics:
  - Agent 框架设计
  - AI 工具化知识工作流
  - Agent 记忆与知识图谱
related_cases: []
related_relations: []
---

# GitHub - Noema

## 一句话总结

Noema 是一个 voice-first desktop AI companion 实验，把语音、记忆、人格 / 情绪、任务 runtime、工具和插件系统组织成桌面陪伴式 agent。

## 当前范围

本页只整理 README 和 GitHub API 元数据；未安装桌面 app，未配置 LLM / Task / TTS / ASR slots，未测试麦克风权限、语音延迟、SQLite 记忆、插件权限或 computer-use / browser-use 能力。

## 摘要

- GitHub 描述为 “A voice-first desktop AI companion with memory, emotion, tools, and plugins.”
- README 把 Noema 描述为类似 JARVIS 的 desktop companion，能以人格化方式说话、记住上下文、理解任务，并通过工具行动。
- 运行结构分成 emotional layer、work layer、interaction layer、output layer、voice pipeline 和 plugin system。
- 功能包括 streaming ASR、VAD、turn detection、Fish Audio TTS、role YAML、conversation memory、task execution runtime、interruption-aware audio path、SQLite 持久记忆和插件系统。
- 插件覆盖 file/search/patch/shell、Electron browser automation、native desktop computer-use、skills manager、MCP manager、sticker expression 和 Fish Audio voice cue。
- GitHub API 抓取时显示 TypeScript 仓库，AGPL-3.0 license，stars 约 88，仓库未归档。

## 当前可支持的判断

- 当前来源支持：Noema 是桌面语音 companion / 本地 agent host 样本，而不是单纯聊天 UI。
- 当前可保守迁出：它补充 [[Agent 框架设计]] 中“agent 运行面会被桌面、语音、任务状态、插件权限和中断处理共同塑形”这一侧。
- 它也补充 [[AI 工具化知识工作流]] 中“AI 工具不一定只是文本/网页工作台，也可能落成持续陪伴式桌面 runtime”。
- 对 [[Agent 记忆与知识图谱]] 的补充较轻：README 只支持 SQLite conversation turns、summaries、user profile 和 task runs 这类持久记忆，不支持图谱层结论。

## 当前边界

- README 的 voice-first 体验、低延迟、turn detection、interrupt、emotion/personality 和 plugin runtime 都未实测。
- `base-tools`、`browser-use`、`computer-use`、`mcp-manager` 等插件可能触达文件、shell、浏览器和桌面控制；后续测试必须隔离权限并检查可撤销性。
- API key、TTS voice id、ASR、代理节点和桌面麦克风权限涉及隐私与凭据安全，当前不写成安装推荐。
- 项目很新且 stars 较少，当前只作为 early sample 保存，不判断维护稳定性。

## 相关主题

- [[Agent 框架设计]]
- [[AI 工具化知识工作流]]
- [[Agent 记忆与知识图谱]]

## 关系

- `补充` -> [[Agent 框架设计]]：提供 voice-first desktop companion runtime 样本。
- `补充` -> [[AI 工具化知识工作流]]：提供桌面陪伴式 AI 工具化形态样本。
- `轻量补充` -> [[Agent 记忆与知识图谱]]：提供 SQLite 持久记忆样本，但未到图谱层。

## 回链

- 对应来源包主文件：[raw/repos/2026-06-09-github-happyfox001-noema/noema.md](../../raw/repos/2026-06-09-github-happyfox001-noema/noema.md)
