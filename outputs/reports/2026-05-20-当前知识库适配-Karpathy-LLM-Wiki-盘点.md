---
type: output
output_type: report
status: reusable
promote_to_wiki: partial
question: 当前 MyLLMWiki 是否已经适配 Karpathy 的 LLM Wiki 思路
scope: 对照 Karpathy LLM Wiki 转述来源中的 raw / wiki / schema / ingest / query / file-back / lint 骨架，盘点当前仓库已有结构、已完成样板和仍需持续观察的缺口
source_pages:
  - 知乎专栏 - Karpathy 的 LLM Wiki 新范式
  - MyLLMWiki
  - 把 MyLLMWiki 跑成可持续增长的个人 LLM Wiki
related_topics: []
related_concepts: []
related_methods:
  - 先把当前状态和伏笔单独记账，再续写长文本
updated: 2026-05-20
---

# 当前知识库适配 Karpathy LLM Wiki 盘点

## 结论

当前 MyLLMWiki 已经阶段性适配 Karpathy 的 LLM Wiki 思路。

它不是完整复刻 Farzapedia，也还缺一手原帖和更多长期使用样本；但就仓库结构和实际运行来说，`raw / wiki / schema / ingest / query / file-back / lint` 这条主骨架已经基本落地。

## 对照 Karpathy 骨架

| Karpathy 口径 | 当前仓库对应层 | 当前状态 |
| --- | --- | --- |
| raw | `Clippings/`、`raw/`、标准来源包 | 已落地。网页、聊天、repo、seed 分流都已经跑过真实样本 |
| wiki | `wiki/sources/`、`wiki/entities/`、`wiki/topics/`、`wiki/methods/`、`wiki/concepts/` | 已落地。来源页、对象页、主题页、方法页、概念页都有正式样板 |
| schema | `AGENTS.md`、`_index/维护协议.md`、模板、skill references | 已落地。页面职责、路由规则、确认边界已经写进控制面 |
| ingest | `Clippings/ -> raw/seeds/todo/wiki/outputs` | 已落地。多轮剪藏、聊天归档和 seed 分流已经按这个路径运行 |
| query | `outputs/reports/`、索引页、问答式盘点 | 已落地。查询结果先落 outputs，再决定是否回写 wiki |
| file-back | 来源页、对象页、目标页、索引、日志的回写 | 已落地。rollout 项目切片、AI coding 样本、机器学习入口等都已回写 |
| lint | `_index/health-check.md`、`_index/待处理.md`、`_index/log.md` | 已落地。健康检查、待处理队列和运行日志已经形成控制回路 |

## 主要适配点

### 1. 不再把知识库当资料堆

当前仓库已经从“保存资料”变成“先保来源，再编译成可导航结构”。

证据是：`raw/` 保原始来源，`wiki/sources/` 保来源摘要，正式抽象只在证据够时进入 topic / method / concept。

### 2. 已经有个人材料入口

Karpathy 口径里最关键的点，不只是公开资料，也包括个人日记、聊天、审美线索和项目语境。

当前仓库已经补出：

- `raw/chats/`：承接聊天与 rollout 归档。
- `wiki/entities/`：承接项目、产品、长期对象。
- `todo/goals/` 和 `todo/tasks/`：承接目标和待办。
- `seeds/inbox/`：承接还没成熟的灵感和高波动线索。

这说明 MyLLMWiki 已经从“资料知识库”升级到了“个人材料也能进系统”的阶段。

### 3. 已经有 file-back 回路

当前查询和整理结果不会只停在一次性回答里。

典型路径是：

```text
来源或问题
-> outputs/reports/
-> wiki/sources / wiki/entities / todo/goals / _index
-> log / health-check / 待处理
```

这和 Karpathy 说的“查询结果继续写回 wiki”方向一致。

### 4. 已经有 lint 控制面

`_index/health-check.md`、`_index/待处理.md` 和 `_index/log.md` 现在共同承担自检职责。

它们能回答：

- 当前结构有没有欠账。
- 哪些来源还需要复核。
- 哪些内容只适合 seed 或 review。
- 最近一次维护到底改了什么。

这让仓库不是只靠记忆续写，而是靠外置状态继续推进。

## 仍需保守的地方

### 1. Karpathy 来源仍是中文二手传播

当前正式来源页已经明确：`知乎专栏 - Karpathy 的 LLM Wiki 新范式` 是方向性补强材料，不是一手原帖。

后续如果要精确讨论 Karpathy 自己的设计口径，仍应补一手来源或实作材料。

### 2. 自动化程度还不高

当前仓库已经有人机协作式 ingest、query、file-back 和 lint，但还不是全自动系统。

这不影响“结构适配”判断，只说明下一步如果追求更像 Farzapedia，需要补自动化脚本、检查器或更稳定的导入流水线。

### 3. 个人对象层还需要继续积累

`MyLLMWiki / WeBox / WhatsBox / Beam` 已经跑出对象样板，但对象层还年轻。

当前最稳判断是：对象层已经成立，但还没有到“所有长期对象都有成熟页”的阶段。

## 阶段性判断

这个目标可以阶段性收口：

- 结构已经对齐 Karpathy LLM Wiki 的核心骨架。
- 新材料分流路径已经跑过多轮真实样本。
- 对象层、行动层、聊天来源页已经从模板进入运行态。
- 控制面能持续记录状态、队列和健康检查。

后续不必再把“是否适配 Karpathy”当作开放待办。

更好的下一步，是按具体项目或具体材料继续运行这套系统：新资料先进 `Clippings/`，不成熟进 `seeds/`，行动项进 `todo/`，稳定知识再回写 `wiki/`。
