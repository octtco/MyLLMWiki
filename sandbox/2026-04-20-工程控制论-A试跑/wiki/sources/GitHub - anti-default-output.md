---
type: source
status: active
source_path: raw/repos/2026-04-15-github-lucent-snow-anti-default-output/anti-default-output.md
source_type: repo_readme
source_url: https://github.com/Lucent-Snow/anti-default-output
source_bundle: raw/repos/2026-04-15-github-lucent-snow-anti-default-output
title: anti-default-output
authors:
  - Lucent-Snow
year: 2026
created_at: 2026-04-15
updated_at: 2026-04-16
temporal_status: evolving
confidence: medium
claim_status: mixed
tags:
  - anti-default-output
  - Skill
  - 输出纠偏
  - 创意输出
  - 默认路径
related_concepts:
  - Skill
  - 反默认输出
  - 默认路径
  - 输出前自检
related_topics: []
---

# anti-default-output

## 一句话总结

`anti-default-output` 是一个把“先识别模型默认生成路径，再有意识偏离它”封装成 skill 的小型仓库，重点不是给一个固定模板，而是建立一套输出纠偏纪律。

## 摘要

- 这是项目仓库的主说明来源，README 和 `SKILL.md` 共同定义了这个项目到底在解决什么问题。
- 仓库把问题讲得很直接：模型天然会滑向高概率、最平均、最安全的输出，而这些输出虽然不一定错，但经常无聊、保守、带明显模板感。
- 这个 skill 的核心机制不是“规定你必须怎么写”，而是要求模型在生成前先自检：自己是不是又在走默认路径。
- 如果判断答案是“是”，就不要直接交出第一版，而要主动换一个更有角度、更有判断、更不那么像套路模板的方向。
- 项目结构也很轻：`SKILL.md` 讲通用方法，`references/` 负责分场景沉淀常见默认错误和偏离方向；当前至少覆盖前端设计和一般写作。
- 从仓库结构看，它更像一个可扩展的“纠偏型 skill”样本，而不只是一次性的 prompt 片段。

## 关键点

- 它把“默认输出”理解成模型工作机制的自然结果，而不是单纯把问题归结为模型偷懒。
- 它既反对 bland 的平均化输出，也反对过度谄媚、永远中庸的回答路径。
- 它的方法论核心是三步：识别默认路径、指出不该继续走的范式、给出可偏离的方向。
- `references/` 的存在很关键，这意味着它可以按场景持续扩展，而不是停留在一句抽象口号。

## 方法拆解

- 它先把问题对象说清楚，也就是 [[默认路径]]：那个最稳妥、最平均、最容易不假思索就交出来的版本。
- 然后要求模型做一次 [[输出前自检]]，在正式生成前先问自己：这是不是所有 AI 都会给出的答案。
- 最后才进入 [[反默认输出]]，也就是有意识地换一个更具体、更有立场、或更不套路的方向。
- 这个顺序很重要，因为它说明仓库讲的不是“写得特别一点”，而是“先识别默认，再决定怎么偏”。

## 证据或原文线索

- README 直接把问题归纳为：AI 默认倾向概率最大的输出，而最平均的输出往往最保守、最没特色。
- `SKILL.md` 明确要求模型在生成前先问自己：“我现在要给出的，是不是那个不假思索就会给出的版本？”
- `SKILL.md` 还把问题进一步拆成两层：一层是高概率路径，一层是偏好对齐带来的谄媚倾向。
- `references/frontend-design.md` 和 `references/writing.md` 都采用“默认错误识别 + 禁止项 + 偏离方向”的结构，说明这个仓库确实在把方法落到具体领域。

## 可直接回证的能力或主张

- 这个项目确实提供了一套可复用的 skill 结构，而不是只有零散提示词。
- 它确实强调生成前自检、负面示例约束、分领域 reference 这三类机制。
- 当前仓库已经把前端设计和写作场景落成了可直接复用的参考文件。
- `SKILL.md` 里的自检问题和偏离方向，足以支撑把“默认路径”和“输出前自检”进一步抽成可复用节点。

## 更偏项目方自述或待验证的判断

- “这样做能稳定产出更高质量内容”目前更像方法主张，还缺更多外部样本支撑。
- README 里对“AI 公司训练得越来越不说人话”这类表述，更适合作为立场背景，不适合直接沉淀成客观结论。
- 这个方法跨多少场景都同样有效，当前也还需要更多来源来验证。

## 我的判断

- 这份来源足以支撑一个稳定概念页，但还不够支撑更高层的主题页。
- 它最值得沉淀的不是“去 AI 味”这种泛化说法，而是“先识别默认路径，再主动偏离”的方法本身。
- 目前最合适的接法，是把它作为 [[Skill]] 的一个纠偏型样本，同时把 [[反默认输出]]、[[默认路径]]、[[输出前自检]] 这几个方法节点显式拆开。

## 相关概念

- [[Skill]]
- [[反默认输出]]
- [[默认路径]]
- [[输出前自检]]

## 相关主题

- 暂无

## 关系

- `支持` -> [[Skill]]：它说明 skill 不只能承载能力扩展，也可以承载输出路径纠偏。
- `定义` -> [[反默认输出]]：当前库里，这个仓库是该概念最直接的一手来源。
- `定义` -> [[默认路径]]：它把模型的高概率第一反应明确视为需要识别的对象。
- `支持` -> [[输出前自检]]：它把生成前自检写成了可复用的执行动作。

## 回链

- 对应原始文件：[raw/repos/2026-04-15-github-lucent-snow-anti-default-output/anti-default-output.md](../../raw/repos/2026-04-15-github-lucent-snow-anti-default-output/anti-default-output.md)
- 对应补充文件：[raw/repos/2026-04-15-github-lucent-snow-anti-default-output/files/SKILL.md](../../raw/repos/2026-04-15-github-lucent-snow-anti-default-output/files/SKILL.md)
- 对应外部来源：[GitHub - Lucent-Snow/anti-default-output](https://github.com/Lucent-Snow/anti-default-output)
