---
date: 2026-05-11
type: seed
status: inbox
seed_type: repo-cluster
source_hint: https://github.com/karpathy/autoresearch
possible_destinations:
  - raw/repos
  - wiki/sources
  - wiki/topics
  - wiki/methods
tags:
  - seeds
  - repo
  - autoresearch
  - agent
  - vibecoding
updated: 2026-05-11
aliases:
  - AutoResearch 自动研究循环线索
---

# AutoResearch 自动研究循环线索

## 原始内容

- [karpathy/autoresearch](https://github.com/karpathy/autoresearch)：Karpathy 的单 GPU 自动研究实验仓库。仓库说明把核心思路写成：给 AI agent 一个小但真实的 LLM 训练设置，让它自动改代码、训练 5 分钟、看指标有没有变好、保留或丢弃改动，然后循环。
- [alvinreal/awesome-autoresearch](https://github.com/alvinreal/awesome-autoresearch)：围绕 autoresearch 风格系统整理的列表，收集 autonomous improvement loops、research agents、autoresearch-style systems。
- 相关 X 链接暂时只保留原地址，正文未抓到：
  - https://x.com/explang_cn/status/2051231673941946538?s=46
  - https://x.com/wy_mask/status/2051332973619040403?s=46
  - https://x.com/weiyux2021/status/2051110798475370702?s=46
  - https://x.com/wadezone/status/2051155060751794328?s=46

## 为什么值得留

- 这条线把 vibecoding 从“一次让模型写代码”往前推了一步：让 agent 围绕一个可度量目标持续实验。
- `program.md` 这种轻量指令文件很像“研究组织的 skill”，它不是直接写业务代码，而是在定义 agent 如何做实验、如何看指标、如何收敛。
- `awesome-autoresearch` 可以作为后续入口，不必一次把所有项目都正式归档。

## 现在的直觉

- 当前更适合先当“自动实验循环”的项目线索保存，不急着抽成正式方法页。
- 对 vibecoding 来说，可迁出的不是 LLM 训练细节，而是这套结构：明确目标指标、限制可编辑范围、短周期运行、记录结果、保留有效改动。
- 如果后面真的要做“是真的吗”或“帮助学习”的原型，也可以借这套循环：让 agent 不只是给答案，而是持续跑验证或练习反馈。

## 可能去向

- `raw/repos`：如果后续要正式保存 `karpathy/autoresearch` 和 `awesome-autoresearch` 的 README 快照。
- `wiki/sources`：如果补成正式来源页，可以先做 `GitHub - autoresearch`。
- `wiki/topics`：如果积累更多同类项目，再考虑整理“自动研究循环”主题。
- `wiki/methods`：只有当这套循环在自己的项目里复用过，再考虑抽方法页。

## 当前不确定点

- X 帖正文未抓到，暂时不能写入它们的具体观点。
- 仓库偏 LLM 训练研究，迁到普通产品开发时需要保守，不应直接写成通用结论。
