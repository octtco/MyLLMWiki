---
type: source
status: review
source_path: raw/web/2026-04-28-linuxdo-topic-2056598-novel-writing-monetization-4/novel-writing-monetization-4.md
source_type: web
source_url: https://linux.do/t/topic/2056598
source_bundle: raw/web/2026-04-28-linuxdo-topic-2056598-novel-writing-monetization-4
title: Linux.do - AI 辅助小说写作赚钱方式（第 4 期）
authors:
  - user2609
created_at: 2026-04-28
updated_at: 2026-04-28
tags:
  - AI写作
  - DeepSeek
  - 交叉校对
related_methods:
  - 先让不同模型交叉找问题，再回写大纲和正文
related_concepts:
  - 输出前自检
  - 反默认输出
related_topics:
  - AI 辅助网文写作
related_relations: []
---

# Linux.do - AI 辅助小说写作赚钱方式（第 4 期）

## 一句话总结

这篇帖最有价值的地方，不是“DeepSeek 很牛”这个判断，而是作者把 Gemini、Codex、CC/DeepSeek 之间的交叉找错顺序讲得更明白了，而且顺手提醒了：检测器的红绿结果本身也不能全信。

## 摘要

- 作者把“大纲先由一个模型生成，再让另一个模型找问题，再把问题带回去修”写成了实际顺序。
- 正文同时给了一个很重要的反例：不要把 AI 检测器的红绿图当最终真相。
- 它更像是第 3 期的加严版：不是只让不同模型轮流写，而是让它们轮流找错和回写。

## 证据或原文线索

- 正文明确写出“Gemini 先生成大纲 -> Codex 找问题 -> DeepSeek 再检查 -> 再回到 Codex”。
- 后半段多次对比不同版本文本和检测图，讨论什么地方被误判成 AI。
- 作者最后直接指出某些检测器的盲点。

## 我的判断

- 当前最稳的部分，是 [[先让不同模型交叉找问题，再回写大纲和正文]] 这条方法继续被实操补强。
- 它还能给 [[输出前自检]] 和 [[反默认输出]] 提供一个写作场景下的补充样本。
- “DeepSeek 一定更好”“某个检测器一定不准”这种结论，这篇帖仍然说不满。

## 当前边界

- 作者自己也承认 DeepSeek 这一环是朋友帮忙搭好，复现条件并不统一。
- 检测器截图只能作为局部现象，不足以当成长期评测标准。

## 相关概念

- [[输出前自检]]
- [[反默认输出]]

## 相关方法

- [[先让不同模型交叉找问题，再回写大纲和正文]]

## 相关主题

- [[AI 辅助网文写作]]

## 关系

- `支持` -> [[先让不同模型交叉找问题，再回写大纲和正文]]：这篇帖把交叉找错顺序写得更清楚。
- `补充` -> [[输出前自检]]：不同模型轮流找问题，本质上是在把自检外包成多轮检查。
- `相关` -> [[反默认输出]]：作者在意的是怎样把机械感和明显 AI 痕迹压下去。

## 回链

- 对应来源包主文件：[raw/web/{spec['bundle']}/{spec['primary']}](../../raw/web/{spec['bundle']}/{spec['primary']})
