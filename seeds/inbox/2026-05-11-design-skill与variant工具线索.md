---
date: 2026-05-11
type: seed
status: inbox
seed_type: tool-cluster
source_hint: https://github.com/jiji262/claude-design-skill
possible_destinations:
  - raw/repos
  - wiki/sources
  - wiki/topics
  - wiki/methods
tags:
  - seeds
  - design
  - skill
  - vibecoding
  - frontend
updated: 2026-05-11
aliases:
  - Design Skill 与 Variant 工具线索
---

# Design Skill 与 Variant 工具线索

## 原始内容

- [jiji262/claude-design-skill](https://github.com/jiji262/claude-design-skill)：一个 portable Claude Skill，把 Claude 引导成 HTML artifacts 设计师，用于 landing page、deck、prototype、animation、poster、wireframe 等。
- 仓库 README 里提到的关键点包括：事实核验优先、品牌资产收集、Advisor mode、输出格式 playbook、多变体策略、反 AI 味设计纪律、浏览器验证。
- [Variant](https://www.variant.art/)：Claude Code presentation canvas 方向的设计工具线索。
- [foryourhealth111-pixel/Vibe-Skills](https://github.com/foryourhealth111-pixel/Vibe-Skills)：一组 all-in-one AI skills package 线索，主打把专家能力和上下文管理封成可复用 skills。
- 相关 X 链接暂时只保留原地址，正文未抓到：
  - https://x.com/ai_xiaomu/status/2049982406942482867?s=46
  - https://x.com/vincentlogic/status/2050031578278252603?s=46
  - https://x.com/mnmn94253156337/status/2050038991416885353?s=46

## 为什么值得留

- 这条线和 vibecoding 很近：用户不是只需要模型“能写页面”，而是需要它更稳定地产出可看的设计资产。
- `claude-design-skill` 的价值不只是 prompt，而是把设计前的核验、资产收集、风格分歧、输出格式、验收步骤都包进 skill。
- Variant 和 design canvas 类工具，可以作为“多方案生成 / 对比 / 迭代”的参考，而不是只让 agent 一次性吐一个页面。

## 现在的直觉

- 这组材料可以先服务“vibecoding 的设计侧”：快速做原型、落地页、deck、交互 mockup。
- `claude-design-skill` 更像流程型工具，Variant 更像画布 / 展示型工具，Vibe-Skills 更像通用 skill 包思路。
- 真正值得验证的是：它们能不能把“AI 默认审美”和“无资产瞎编”这两个问题压住。

## 可能去向

- `raw/repos`：如果后续正式保存 `claude-design-skill`、`Vibe-Skills` 的 README 快照。
- `wiki/sources`：可以分别补 `GitHub - claude-design-skill`、`GitHub - Vibe-Skills`。
- `wiki/topics`：如果积累更多样本，可整理“AI 设计 skill 化”主题。
- `wiki/methods`：如果自己项目中验证有效，可抽“先收集真实资产，再生成设计变体”这类方法。

## 当前不确定点

- Variant 的具体能力需要后续用网页或实际产品进一步确认。
- X 帖正文未抓到，不能写入具体观点。
- `claude-design-skill` 的真实效果需要跑一个 vibecoding 设计任务来验证。
