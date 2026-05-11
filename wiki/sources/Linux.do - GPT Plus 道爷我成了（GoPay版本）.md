---
type: source
status: review
source_path: raw/web/2026-04-29-linuxdo-topic-2079271-gpt-plus-gopay-case/gpt-plus-gopay-case.md
source_type: web
source_url: https://linux.do/t/topic/2079271
source_bundle: raw/web/2026-04-29-linuxdo-topic-2079271-gpt-plus-gopay-case
title: Linux.do - GPT Plus 道爷我成了（GoPay版本）
authors:
  - zzzxdm
created_at: 2026-04-29
updated_at: 2026-04-29
tags:
  - gpt-plus
  - GoPay
  - 风险来源
related_concepts: []
related_topics: []
related_relations: []
---

# Linux.do - GPT Plus 道爷我成了（GoPay版本）

## 一句话总结

这是一篇个人操作回报帖：作者声称自己通过 WhatsApp、Talkatone 和 GoPay 走通了 GPT Plus 开通流程，还贴了一个直跳 checkout 的脚本，但当前更适合作为一次性样本保存，而不是稳定路径说明。

## 摘要

- 正文先明确感谢另外两条讨论串，再把自己的操作过程压成 4 步：装 WhatsApp 和 GoPay、接码注册、开通 GPT Plus、再补一个 checkout 直达脚本。
- 作者说 `+86` 手机号收不到 WhatsApp 验证码，于是改用 Talkatone 美国号；GoPay 注册也继续沿用这个号。
- 帖子附了一个 bookmarklet，核心做法是读取当前 ChatGPT 登录态，然后向支付接口发起一次带 `country=ID`、`currency=IDR` 的 checkout 请求。
- 评论区里又补了一条经验判断：作者自称没有使用印尼节点，而是用日本 IP 也走通了。
- 当前更稳的保存方式，是把它看成“同簇社区里出现过的一次个人成功回报 + 一段脚本样本”，而不是把它当成已验证的普适教程。

## 证据或原文线索

- 正文逐条列出 WhatsApp、Talkatone、GoPay 和 GPT Plus 的串联顺序，说明这是一次操作回放，不只是转述别人的结论。
- 帖子直接附上了 bookmarklet，脚本里把 `country` 写成 `ID`、`currency` 写成 `IDR`，还显式请求 `checkout_session_id`。
- 评论区有人追问“要不要印尼节点”，作者的直接回答是“不用什么印尼节点……我是日本的 IP”。
- 结尾还把体验压成“全程不要一分钱，接码都省了”“不需要印尼节点”，这是当前最需要保守处理的两句结论。

## 我的判断

- 这份来源当前只适合作为一次性个人操作样本和脚本样本保存。
- 当前能较稳保留下来的，不是这段脚本现在仍然可用，而是社区里确实出现过一种“通过前端登录态直跳印尼区 checkout”的尝试路径。
- 关于 Talkatone 接码可行性、是否真的不需要印尼节点、是否可以 0 成本走通，以及脚本还能否触发同样的 checkout 流程，后续都需要更多交叉来源验证。

## 相关概念

- 暂无

## 相关主题

- 暂无

## 关系

- `补充` -> [[Linux.do - GPT Plus 开通新方法]]：两篇都围绕 GoPay 这条线，但这篇更像个人实操回报和脚本样本。
- `待验证` -> checkout 直跳脚本：脚本中涉及的支付接口、区域参数和优惠活动标识都具有明显时效性。
- `待验证` -> 区域与成本判断：帖中关于“不需要印尼节点”“全程不要一分钱”的说法当前都缺稳定复现证据。

## 回链

- 对应来源包主文件：[raw/web/2026-04-29-linuxdo-topic-2079271-gpt-plus-gopay-case/gpt-plus-gopay-case.md](../../raw/web/2026-04-29-linuxdo-topic-2079271-gpt-plus-gopay-case/gpt-plus-gopay-case.md)
- 对应元数据：[raw/web/2026-04-29-linuxdo-topic-2079271-gpt-plus-gopay-case/metadata.json](../../raw/web/2026-04-29-linuxdo-topic-2079271-gpt-plus-gopay-case/metadata.json)
- 对应外部来源：[Linux.do 讨论串](https://linux.do/t/topic/2079271)
