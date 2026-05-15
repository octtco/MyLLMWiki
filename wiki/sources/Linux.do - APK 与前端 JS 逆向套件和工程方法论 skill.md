---
type: source
status: review
source_path: raw/web/2026-05-15-linuxdo-topic-2142539-reverse-engineering-skill/reverse-engineering-skill.md
source_type: web
source_url: https://linux.do/t/topic/2142539
source_bundle: raw/web/2026-05-15-linuxdo-topic-2142539-reverse-engineering-skill
title: Linux.do - APK 与前端 JS 逆向套件和工程方法论 skill
authors:
  - hisence
created_at: 2026-05-15
updated_at: 2026-05-15
temporal_status: volatile
confidence: medium
claim_status: review
tags:
  - Reverse Engineering
  - Skill
  - Security Research
related_methods: []
related_concepts:
  - Skill
related_topics: []
related_cases: []
related_relations: []
---

# Linux.do - APK 与前端 JS 逆向套件和工程方法论 skill

## 一句话总结

这篇帖提供的是一组逆向工程工具和配套 skill 线索，价值在于观察“专业工具链 + AI skill”如何被组合成工作流；但由于具备明显双用途风险，本库只保守保存来源和结构，不扩写可滥用操作步骤。

## 当前范围

本页只整理来源定位、工具类型和知识库落点，不复述破解、绕过、接口探测等可操作细节。

## 摘要

- 来源列出 APK 静态分析、解包签名、动态 hook、前端 JS 逆向、浏览器自动化和二进制分析相关工具。
- 帖子还提供了一组自用 skill 包，包括 APK 分析、JS 逆向、IDA、radare2 和综合逆向工作流。
- 对这座知识库来说，更稳的抽取点是：复杂技术工作可以被拆成工具链、方法纪律和 skill 包。
- 由于材料涉及逆向、抓包、破解接口等高风险语境，当前只进入 `review`，不提升为正式方法页。

## 证据或原文线索

- 原帖链接：`https://linux.do/t/topic/2142539`
- 原文提到 `anything-analyzer`、`js-reverse-mcp`、`ida-pro-mcp`、`playwright-mcp`、`jadx`、`Apktool`、`frida`、`radare2` 等工具类别。
- 原文提到配套 `skills.zip`，含多个逆向相关 skill。

## 当前可支持的判断

- 当前来源支持：在高复杂度技术任务中，skill 可能承载“工具选择 + 工作流纪律 + 检查路径”，而不是单条 prompt。
- 当前可保守迁出：这类 skill 更适合在合法授权、安全研究、CTF 或自有资产分析场景下讨论。

## 当前边界

- 不把这篇帖整理成逆向教程。
- 不保存或扩写破解、绕过、未授权访问、接口滥用等具体动作。
- 附件 skill 未本地化和审计前，不评价其质量。

## 相关概念

- [[Skill]]

## 关系

- `支持` -> [[Skill]]：提供一个工具链型 skill 包样本。
- `待验证` -> [[Skill]]：附件内容未审计，不能直接视为稳定可复用 skill。

## 回链

- 对应原始文件：[raw/web/2026-05-15-linuxdo-topic-2142539-reverse-engineering-skill/reverse-engineering-skill.md](../../raw/web/2026-05-15-linuxdo-topic-2142539-reverse-engineering-skill/reverse-engineering-skill.md)
