# 运行日志

这里记录比较重要的 ingest、compile、query、回写和修补动作。

建议每次只记短条目，重点放在“做了什么”和“下一步是什么”。

## 2026-05-20

- 新增 [[2026-05-20-当前知识库适配-Karpathy-LLM-Wiki-盘点]]，对照 `raw / wiki / schema / ingest / query / file-back / lint` 盘点当前仓库与 Karpathy LLM Wiki 思路的适配情况
- 将“确认当前知识库适配卡帕西吗”标记为完成，并把 [[把 MyLLMWiki 跑成可持续增长的个人 LLM Wiki]] 从 `active` 收口为 `done`
- 按用户确认，将 vApp 下载安装卡住 / 推送开关状态异常任务，以及语音对话反应时间和语种匹配任务标记为完成
- 同步更新 [[目标索引]]、[[总览]] 与 [[health-check|健康检查]]，把输出页数量从 19 调整为 20

## 2026-05-22

- 新增 7 条待办：微盒首页 / 发现页信息流广告高度问题、微盒和 WhatsBox 断网首次启动网络弹窗循环问题、BotBuddy、Tether、Tandem、Speakr、scordcard 更换模版
- 新增 [[任务总览]]，把 `todo/tasks/` 当前任务整理成未完成、状态不一致、已完成三块；同时将正文已勾选的 `Tandem` 和 `Speakr` 同步为 `done`
- 将 [[待办事项.base]] 改成主任务操作台，增加“未完成 / 已完成 / 全部任务”三个可编辑视图；[[任务总览]] 改为说明入口，不再维护静态清单
- 按用户确认，将 [[任务总览]] 改成唯一待办页并按时间分组；删除 `todo/tasks/` 下旧的单任务页，[[待办事项.base]] 改为入口视图

## 2026-04-22

- 将旧的 `wiki/`、`_index/`、`outputs/` 和 `首页.md` 备份到 `_rebuild_backups/2026-04-22-full-rerun/`
- 只保留 `raw/` 与 `Clippings/` 作为原始来源层，按新规则从零重建知识库
- 重新建立 9 篇来源页，覆盖当前仓库里的全部正式来源包
- 基于这些来源重新筛出 12 个概念页和 3 个主题页
- 重建来源索引、概念索引、主题索引、待处理、健康检查、总览和首页
- 参照最新 skill 与 `outputs/reports/` 里的 v0.2 规程，补齐 `wiki/methods/`、`wiki/cases/`、`wiki/domains/` 目录占位和模板
- 新增 [[方法索引]]，并统一 `首页`、[[总览]]、[[维护协议]]、`wiki/README.md`、`outputs/README.md` 的最新版结构口径
- 把 `outputs/` 明确恢复为“工作层 + 任务结果层”，修正“输出页数量为 0”这类旧口径遗留
- 为 [[工程控制论（第三版）]] 新建 `outputs/reports/2026-04-22-工程控制论-长文拆解工作层/`，补齐范围骨架、章节工作卡、候选池与 page-type screening、review gate
- 正式新增 6 篇《工程控制论》方法页、5 篇新概念页，并重写对应来源页、主题页和 3 篇旧概念页
- 更新方法索引、概念索引、主题索引、来源索引、待处理、健康检查、总览和首页，使《工程控制论》这条长材料链回到完整的 longform workflow
- 继续把《工程控制论》3-19 章重组为四个中层问题簇，其中“不确定性、信息不完备和可靠性”这一团正式升成 [[先把不确定性并入控制问题]]
- 更新 `outputs/reports/2026-04-22-工程控制论-长文拆解工作层/04-中段问题簇.md`，并把其余三团暂留工作层，避免再拆回技术目录
- 继续把《工程控制论》3-19 章补成逐章细卡、全书终筛和终版 review gate，补齐 `05`、`06`、`07` 三张工作层子卡
- 再为《工程控制论》新增 3 篇方法页和 12 篇概念页，把中段技术簇和后段不确定性簇正式接回 `wiki/`
- 统一回写来源页、主题页、方法页、索引、待处理、健康检查、总览和首页，让这条长材料链在控制面上收口到 `10 方法 / 20 概念 / 8 张工作层子卡`

## 2026-04-23

- 调整主题页写法：方法页不再在主题页正文外单列成平行板块，而是优先嵌进正文第一次真正需要它的位置
- 同步更新 `wiki/_templates/主题页模板.md`，改成“正文自然调用方法；页尾如需补导航，只留一句轻补”
- 重写 [[控制论式系统思维]] 的中段推进方式，去掉独立的“相关方法”分节
- 更新 `myllmwiki-steward` skill 的方法页规则：方法页不只讲卡点与调用时机，还要讲这一步到底在做什么、最小动作和至少一个具体案例
- 同步更新 `wiki/_templates/方法页模板.md`，把方法页模板升级到 `卡点 / 错法 / 这一步在做什么 / 最小动作 / 调用时机 / 最小案例 / 已出现的具体用法 / 变形 / 边界` 这套结构
- 先拿 [[先定义评价标准，再谈优化]] 和 [[先把不确定性并入控制问题]] 两篇方法页做 v2 实改，补进最小动作、最小案例和库内具体用法切片
- 再把其余 8 篇《工程控制论》方法页全部升级到 v2 结构，让整组方法页都具备“这一步在做什么 / 最小动作 / 最小案例 / 已出现的具体用法”

## 2026-04-24

- 新增 `outputs/reports/2026-04-24-个人-LLM-Wiki-结构升级方案-v0.2.md`，把“聊天 / 灵感 / 目标 / 待办”如何接入现有知识库结构整理成一份升级方案稿，并明确后续优先补 `entities` 与 `goals` 两层
- 新增 `outputs/reports/2026-04-24-个人-LLM-Wiki-模板与路由细则-v0.3.md`，把聊天来源页、对象页、目标页和 seed 页的初版模板，以及“新材料先进哪一层”的路由细则单独落成执行补层
- 新增 `raw/chats/`、`wiki/entities/`、`todo/goals/` 三个正式落点，补齐聊天来源页、对象页、目标页与灵感种子模板，并同步改写首页、总览、协议和各层 README，让“聊天 / 对象 / 目标 / 待办”的接入规则正式进仓库口径
- 把 `Clippings/` 正式升级成统一收件箱，新加 `Clippings/README.md`，并同步改写协议、总览、首页、`raw/README.md`、`seeds/README.md`，让“所有原始资料先进 Clippings，再由维护流程分流”成为仓库默认入口

## 2026-04-27

- 清空这一轮 `Clippings/` 里的 5 篇网页剪藏：规范化到 `raw/web/` 来源包，新增 5 篇来源页，并把高时效代理 / 试用号帖挂到 review，把 Karpathy LLM Wiki 与两篇焚决 / 风格 Prompt 帖接回正式来源层。
- 继续处理 `seeds/inbox/` 的 5 张种子卡：把 `404 Media`、`Futurism`、`Malus.sh` 和 `agent_java_offer` 迁成正式来源包与来源页，把 `Grok 镜像站` 明确保留为高波动入口线索

## 2026-04-28

- 处理 `Clippings/2026_副本/`：把 203 个 Codex rollout 聊天日志整体迁入 `raw/chats/2026-02-to-2026-04-codex-rollout-archive/`，保留原 `.jsonl` 目录树，补 `metadata.json`、`inventory.md` 和一篇批次级聊天来源页

- 校正 `$myllmwiki-steward` skill 与核心 reference：把 `Clippings/` 明确为统一收件箱，并把 `seeds/`、`todo/`、`raw/chats/`、`raw/books/`、对象页、目标页、聊天来源页这些新版结构正式写回 skill 路由
- 新增 [[对象索引]]、[[目标索引]]，并同步更新 [[总览]]、[[维护协议]]、[[health-check|健康检查]] 与首页，让对象层 / 目标层从“只有目录和模板”进一步补到可浏览的控制面


- 清空这一轮 `Clippings/` 里的 7 篇 Linux.do 小说写作系列帖子：规范化到 `raw/web/` 来源包，并新增 7 篇对应来源页
- 基于这组新来源补出主题页 [[AI 辅助网文写作]]，以及 3 条方法页：[[先按平台和榜单反推样本，再定自己的写法]]、[[先把当前状态和伏笔单独记账，再续写长文本]]、[[先让不同模型交叉找问题，再回写大纲和正文]]
- 为项目本体补出第一篇正式对象页 [[MyLLMWiki]] 和第一篇正式目标页 [[把 MyLLMWiki 跑成可持续增长的个人 LLM Wiki]]，并新增任务“按项目切分 rollout 聊天归档并补对象目标样板”
- 把 `Clippings/` 里这条只保留到评论层的 Linux.do 生图入口剪藏改分流到 `seeds/inbox/2026-04-28-chatgpt2api-无限生图入口线索.md`，明确它现在只是高波动入口线索，不先误写成正式来源页
- 从 [[Codex rollout 历史聊天归档（2026-02 至 2026-04）]] 里切出第一份项目级子归档 [[Codex rollout - MyLLMWiki 项目切片（2026-04-13 至 2026-04-23）]]，并回写到 [[MyLLMWiki]]、[[把 MyLLMWiki 跑成可持续增长的个人 LLM Wiki]] 与相关控制面
- 再从 rollout 总归档里切出 [[Codex rollout - WeBox 项目切片（2026-03-10 至 2026-04-24）]] 和 [[Codex rollout - WhatsBox 项目切片（2026-02-26 至 2026-04-17）]]，并补出 [[WeBox]]、[[WhatsBox]] 两篇对象页，让聊天项目样板从 1 条扩成 3 条
- 继续从 rollout 总归档里切出 [[Codex rollout - Beam 项目切片（2026-03-19 至 2026-04-17）]]，并补出 [[Beam]] 对象页；同时把 `Somnus` 暂留在待评估状态，因为当前 7 个 session 里噪声偏多

## 2026-04-29

- 清空这一轮 `Clippings/` 里的 2 篇 GoPay / GPT Plus 论坛经验帖：规范化到 `raw/web/2026-04-29-linuxdo-topic-2076911-gpt-plus-gopay-method/` 和 `raw/web/2026-04-29-linuxdo-topic-2079271-gpt-plus-gopay-case/` 两个来源包
- 新增两篇对应来源页 [[Linux.do - GPT Plus 开通新方法]]、[[Linux.do - GPT Plus 道爷我成了（GoPay版本）]]，继续按高时效风险样本口径写成 `review`，不提前抽方法页或概念页
- 更新 [[来源索引]]、[[待处理]]、[[总览]]、[[health-check|健康检查]] 和首页，并把收件箱原件从 `Clippings/` 移除

## 2026-05-09

- 清空这一轮 `Clippings/` 里的 3 篇新网页剪藏：迁入 `raw/web/2026-04-29-linuxdo-topic-2082533-seedance-director-thinking/`、`raw/web/2026-04-30-linuxdo-topic-2086346-home-broadband-relay-node/` 和 `raw/web/2026-05-09-linuxdo-topic-2138957-student-entrepreneurship-10-obstacles/` 三个来源包
- 新增对应来源页 [[Linux.do - Seedance 2.0 结合 GPT 的导演思维教学]]、[[Linux.do - 自建家宽节点与中转站部署教程]]、[[Linux.do - 学生创业的 10 道坎]]，这轮继续全部按 `review` 口径保存，不提前上提成方法页或主题页
- 复核 `seeds/inbox/` 里的 `Grok 镜像站`、`ChatGPT2API 无限生图入口线索`、`gpt-pp-team 待研究仓库` 三张卡，本轮继续保留为高波动入口或待研究仓库，不误升正式来源
- 同步更新 [[来源索引]]、[[待处理]]、[[总览]]、[[health-check|健康检查]] 和运行日志，并把已完成迁移的收件箱原件从 `Clippings/` 移除
- 再把 [[AI 辅助网文写作]] 这组里更稳的部分正式往上提：重写主题页主线，强调“平台样本校准 -> Skill 外置 -> 状态记账 -> 多模型交叉找问题”这条生产链，并把 3 条相关方法页从 `review` 提到 `active`

## 2026-05-11

- 将用户提供的一批 vibecoding / autoresearch / design skill / 订阅价格入口线索先整理进 `seeds/inbox/`：新增 [[2026-05-11-autoresearch-自动研究循环线索|AutoResearch 自动研究循环线索]]、[[2026-05-11-vibecoding-是真的吗与帮助学习方向|Vibecoding：是真的吗与帮助学习两个方向]]、[[2026-05-11-design-skill与variant工具线索|Design Skill 与 Variant 工具线索]]、[[2026-05-11-订阅共享与区价入口线索|订阅共享与区价入口线索]]
- 明确 `是真的吗`、`帮助学习` 是用户准备 vibecoding 的两个项目方向，不抽象成概念页；后续优先进入目标页、任务页或项目对象页
- 保留 X 链接为待补正文状态，并在 [[待处理]] 登记后续回填任务；高波动渠道和价格入口只作为 seed 保存，不写成稳定方法
- 新增 [[2026-05-11-product-hunt-产品发现与发布入口|Product Hunt 产品发现与发布入口]]，把它先作为 vibecoding 的产品灵感、竞品观察和未来发布入口保存，并在 [[待处理]] 登记一次相关产品观察任务

## 2026-05-15

- 将 Trellis 中文文档、`mattpocock/skills` 的 `grill-me`、以及两篇 Linux.do 使用帖整理成 4 个来源包和 4 篇来源页：[[Trellis Doc - 中文文档]]、[[GitHub - grill-me]]、[[Linux.do - 大道至简的胜利，一个神级 skill 推荐]]、[[Linux.do - Trellis + grill-me 组合用起来很爽]]
- 新增方法页 [[先追问到共享理解，再进入任务执行]]，把 `grill-me + Trellis` 保守整理为“前置澄清 skill + 结构化执行框架”的组合样本
- 回写 [[AI coding framework]] 与 [[Skill]]，强调 skill 不只承载执行能力，也可以承载任务进入框架前的澄清纪律；同时保留“社区体验不等于普遍 benchmark”的边界
- 继续把 [[GitHub - MetaGPT]]、[[GitHub - awesome-ai-dev-prompts]] 和 [[GitHub - awesome-ai-software-development-agents]] 整理成 3 个 repo 来源包和 3 篇来源页；回写 [[Agent 框架设计]] 与 [[AI coding framework]]，区分多角色 SOP 框架、prompt 资料库和 agent 生态导航表
- 清空 `Clippings/` 剩余 3 篇剪藏：新增 [[Linux.do - APK 与前端 JS 逆向套件和工程方法论 skill]]、[[Linux.do - 自建科学上网教程]]、[[Linux.do - CPA 与 New API 中转站搭建教程]]，全部保持 `review`，只保存来源结构和风险边界，不扩写逆向、翻墙或 API 中转操作指南
- 继续整理 3 篇新剪藏：新增 [[Linux.do - 简论机器学习前言]]、[[Linux.do - 机器学习之前，先学会看数据]]、[[Linux.do - 产品经理、客户经理以及技术头儿有什么区别]]；两篇机器学习来源合并支撑 `review` 主题 [[机器学习工程入口]]，角色辨析来源先不升方法页

## 2026-05-18

- 复核一批“周报式 AI 大事”口径，只把能确认真实存在、且值得继续跟的部分留下来，不把二手传播里的“最强 / 王炸 / 完全自主 / 本质一样”直接写进正式知识页
- 回写 [[AI coding framework]]：补进 `Codex / Gemini / WebBridge` 这条“系统级操作代理 + 浏览器控制桥”主线，区分完整框架、系统内置代理方向和浏览器操作基础设施
- 回写 [[Agent 框架设计]]：补进 `TRINITY` 与 `AutoScientist` 这条“协调器 / 自动实验系统”主线，保守区分多角色 SOP、动态编排和窄边界研究自动化
- 在 `seeds/inbox/` 新增 [[2026-05-18-实时多模态交互线索|实时多模态交互线索]]、[[2026-05-18-多模态生成能力簇线索|多模态生成能力簇线索]]、[[2026-05-18-麻醉语言预测与AI类比待验证|麻醉语言预测与 AI 类比待验证]] 三张种子卡，接住暂不适合直接升正式来源页的高波动线索
- 更新 [[主题索引]]、[[待处理]] 和运行日志，把后续需要补正式来源页、补对照来源和筛代表样本的工作挂回控制面

## 2026-05-19

- 为 `Codex / Gemini / WebBridge / TRINITY / AutoScientist` 新建 5 个最小来源包和 5 篇正式来源页，先把 topic 背后的外部样本接回 `raw/web/` 与 `wiki/sources/`
- 回写 [[AI coding framework]] 与 [[Agent 框架设计]]，把上轮正文里的外部链接换成正式来源页回链，并同步更新主题索引
- 更新 [[来源索引]]、[[总览]]、[[health-check|健康检查]]、[[待处理]] 和运行日志，把计数、观察点和下一步动作重新对齐到当前仓库状态

## 2026-05-21

- 整理 Hive 资料簇：把项目页迁入 `raw/web/2026-05-21-cslikai-hive/`，把 GitHub README 保存到 `raw/repos/2026-05-21-github-jusperlee-hive/`，把用户放入 `Clippings/` 的 arXiv PDF 复制进 `raw/papers/2026-01-30-arxiv-2601-22599-hive/`
- 新增来源页 [[CSLikAI - Hive 项目页]]、[[GitHub - Hive]]、[[arXiv - Hive 数据集论文]]，并补出对象页 [[Hive]]
- 新增主题页 [[音频分离数据集与监督纯度]]，把 Hive 保守整理为“监督信号纯度影响数据效率”的音频分离样本；同时轻量回写 [[机器学习工程入口]]
- 更新 [[来源索引]]、[[对象索引]]、[[主题索引]]、[[待处理]] 和 [[总览]]；Hugging Face dataset card 本轮连接失败，先作为后续可补边界保留

## 2026-05-25

- 整理用户近期关注的 16 条 GitHub 仓库线索：12 个可访问仓库迁入 `raw/repos/2026-05-25-github-*`，保留 README 快照和基础 metadata
- 新增 12 篇来源页：[[GitHub - anthropic-cookbook]]、[[GitHub - awesome-chatgpt-prompts]]、[[GitHub - Bytebot]]、[[GitHub - rrweb]]、[[GitHub - Understand Anything]]、[[GitHub - CodeGraph]]、[[GitHub - AI Engineering from Scratch]]、[[GitHub - FinceptTerminal]]、[[GitHub - andrej-karpathy-skills]]、[[GitHub - Presenton]]、[[GitHub - knowledge-work-plugins]]、[[GitHub - Multica]]
- 新增主题页 [[代码库图谱化理解]] 与 [[AI 工具化知识工作流]]，并回写 [[AI coding framework]]、[[Agent 框架设计]]、[[机器学习工程入口]]
- 将 `learn-anything/anisora`、`ohmybrew/oh-my-pi`、`sherlock-audit/claude-plugins-official`、`zebbern/free-claude-code` 四个当前 404 仓库名保存为 seed；`nari-labs/multica` 当前 404，但已用可访问的 [[GitHub - Multica]] 承接
- 更新 [[来源索引]]、[[主题索引]]、[[待处理]] 和 [[总览]]
- 补入 `alexpate/awesome-design-systems` 与 Apple HIG：新增两个来源包、两篇来源页和主题页 [[设计系统与平台规范]]；Apple HIG 页面保留官方 DocC JSON 快照，awesome list 保留 README 原文快照
- 将 `Clippings/` 中的 `book-en-print.pdf` 与 `book-zh-print.pdf` 迁入 `raw/books/2026-05-25-prompts-chat-the-prompting-book/`，作为 [[The Prompting Book]] 的中英双语书籍来源包保存
- 新增 `outputs/reports/2026-05-25-The-Prompting-Book-长书拆解工作层/`，补出范围骨架、章节工作卡、候选池与 page-type screening，暂不把 CoT、few-shot、context engineering 等章节标题硬升概念页
- 新增来源页 [[The Prompting Book]] 与主题页 [[提示词设计]]，并轻量回写 [[AI 工具化知识工作流]]、[[AI coding framework]]、[[Skill]] 和 [[GitHub - awesome-chatgpt-prompts]]
- 清空 `Clippings/` 当前有效资料：核对 `2601.22599v1.pdf` 与 Hive 论文包内 PDF hash 一致后移除重复件；迁入两篇 Linux.do 剪藏，新增来源页 [[Linux.do - GPT Image 2.0 生图 50 种风格速查表]] 和 [[Linux.do - AI 产品经理简历与面试建议]]
- 补齐 5 个 `raw/web/2026-05-19-*` 最小快照来源包的 `metadata.json`，并同步更新 [[提示词设计]]、[[来源索引]]、[[主题索引]]、[[总览]]、首页与 [[health-check|健康检查]]

## 2026-05-28

- 整理用户新关注的 6 条 GitHub 仓库线索：[[GitHub - Sim]]、[[GitHub - MarkItDown]]、[[GitHub - Open Deep Research]]、[[GitHub - ChinaTextbook]]、[[GitHub - system-design-primer]]、[[GitHub - MindsDB]]
- 新增 6 个 `raw/repos/2026-05-28-github-*` 来源包，保留 README 快照、标准 `metadata.json` 和完整 `github-api.json`
- 回写 [[Agent 框架设计]] 与 [[AI 工具化知识工作流]]，新增主题页 [[系统设计学习入口]]
- 对 [[GitHub - ChinaTextbook]] 保持 `review`：只保存来源入口，不下载教材 PDF，不处理为可复用教材包

## 2026-05-29

- 整理用户新关注的 4 条 GitHub 仓库线索：[[GitHub - NewsNow]]、[[GitHub - developer-roadmap]]、[[GitHub - Hyperswitch]]、[[GitHub - Graphiti]]
- 新增 4 个 `raw/repos/2026-05-29-github-*` 来源包，保留 README 快照、标准 `metadata.json` 和完整 `github-api.json`
- 新增主题页 [[开发者学习路线图]] 与 [[Agent 记忆与知识图谱]]
- 回写 [[Agent 框架设计]]、[[AI 工具化知识工作流]]、[[系统设计学习入口]] 与 [[机器学习工程入口]]；Hyperswitch 和 NewsNow 先只保留来源页，不强行升主题

## 2026-06-01

- 整理用户新关注的 12 条 GitHub 仓库线索：其中 [[GitHub - NewsNow]]、[[GitHub - developer-roadmap]] 已存在，未重复入库
- 新增 8 个 repo 来源包和来源页：[[GitHub - RSSHub]]、[[GitHub - AI Hedge Fund]]、[[GitHub - JavaScript Algorithms]]、[[GitHub - MoneyPrinterTurbo]]、[[GitHub - Harness]]、[[GitHub - Scrapling]]、[[GitHub - github docs]]、[[GitHub - Supermemory]]
- 新增主题页 [[信息源订阅与内容聚合]]、[[AI 金融研究工具]]、[[算法与数据结构学习入口]]
- 将 `lumina-ai-inc/hermes-webui` 与 `Mbed-TLS/ECC` 两个 404 仓库名保存为 seed，等待准确 URL
- 回写 [[AI 工具化知识工作流]] 与 [[Agent 记忆与知识图谱]]；金融、scraping 和短视频自动化相关来源全部保持 `review`

## 2026-06-02

- 整理用户新关注的 5 条 GitHub 仓库线索：[[GitHub - Scrapling]] 已存在，未重复入库
- 新增 4 个 repo 来源包和来源页：[[GitHub - Impeccable]]、[[GitHub - Compound Engineering]]、[[GitHub - TradingAgents]]、[[GitHub - revfactory Harness]]
- 回写 [[AI coding framework]]、[[Agent 框架设计]]、[[AI 工具化知识工作流]]、[[AI 金融研究工具]] 与 [[设计系统与平台规范]]
- TradingAgents 继续按金融研究样本保存，不提供投资建议；revfactory Harness 与已有 [[GitHub - Harness]] 明确区分来源和定位

## 2026-06-03

- 整理用户新关注的 6 条 GitHub 仓库线索：[[GitHub - Supermemory]] 已存在，未重复入库
- 新增 5 个 repo 来源包和来源页：[[GitHub - ECC]]、[[GitHub - Flowsint]]、[[GitHub - VoxCPM]]、[[GitHub - Machine Learning for Trading]]、[[GitHub - Production Agentic RAG Course]]
- 新增主题页 [[OSINT 与图谱化调查]] 与 [[语音生成与音频模型]]
- 回写 [[AI coding framework]]、[[Agent 框架设计]]、[[AI 工具化知识工作流]]、[[Agent 记忆与知识图谱]]、[[AI 金融研究工具]] 与 [[机器学习工程入口]]
- Flowsint、VoxCPM、Machine Learning for Trading 均保持 `review`：分别保留 OSINT 伦理 / 隐私、声音克隆授权、金融非投资建议边界

## 2026-06-04

- 整理用户新关注的 GitHub 仓库线索：[[GitHub - Aegis]]
- 新增 `raw/repos/2026-06-04-github-ganyuanran-aegis/` 来源包，保留 README 快照、`github-api.json` 和 `metadata.json`
- 新增来源页 [[GitHub - Aegis]]，并回写 [[AI coding framework]] 与 [[Agent 框架设计]]
- Aegis 先作为 method-pack / workflow discipline 样本保存，不写成 runtime、daemon 或最终完成判定器

## 2026-06-05

- 整理用户新关注的 GitHub 仓库线索：[[GitHub - gstack]]
- 新增 `raw/repos/2026-06-05-github-garrytan-gstack/` 来源包，保留 README 快照、`github-api.json` 和 `metadata.json`
- 新增来源页 [[GitHub - gstack]]，并回写 [[AI coding framework]] 与 [[Agent 框架设计]]
- gstack 先作为角色化 AI coding skill stack / 虚拟工程团队流程样本保存；setup、team mode、浏览器、iOS QA、deploy、安全审计和多 host 行为后续再做隔离验证
- 整理用户新关注的 GitHub 仓库线索：[[GitHub - fishkeeper]]
- 新增 `raw/repos/2026-06-05-github-frankhuy-fishkeeper/` 来源包，保留 README 快照、`github-api.json` 和 `metadata.json`
- 新增来源页 [[GitHub - fishkeeper]]，并回写 [[AI 工具化知识工作流]]
- fishkeeper 先作为闲鱼 / 闲管家开放平台的垂直业务 API skill 样本保存；真实店铺 API 调用、订单操作、平台授权和凭据安全后续再复核

## 2026-06-08

- 整理用户新关注的 17 条 GitHub 仓库线索：10 个可访问仓库迁入 `raw/repos/2026-06-08-github-*`，保留 README 快照、`github-api.json` 和 `metadata.json`
- 新增 10 篇来源页：[[GitHub - Prompt Engineering Interactive Tutorial]]、[[GitHub - kanata]]、[[GitHub - node-clinic]]、[[GitHub - Vanna]]、[[GitHub - PraisonAI]]、[[GitHub - AIHawk]]、[[GitHub - MCP Toolbox for Databases]]、[[GitHub - open-notebook]]、[[GitHub - goose]]、[[GitHub - whisper.cpp]]
- 回写 [[AI coding framework]]、[[Agent 框架设计]]、[[AI 工具化知识工作流]]、[[提示词设计]]、[[语音生成与音频模型]] 与 [[机器学习工程入口]]
- 将 7 个 GitHub API 当前返回 Not Found 的仓库名保存为 seed：`YangLing0818/better-sqlite3`、`Arrowana/WPPluginMaker`、`Crosstalk-Solutions/OpenVPN`、`Leonxlnx/Moxin`、`mvanhorn38/bughunt`、`NousResearch/l1`、`yikart/parseable`
- Vanna、MCP Toolbox、AIHawk、OpenVPN / bughunt 线索等都保持 `review` 或 seed：数据库、求职自动化、网络部署和安全相关内容不迁出操作教程

## 2026-06-09

- 整理用户新关注的 GitHub 仓库线索：[[GitHub - Noema]]
- 新增 `raw/repos/2026-06-09-github-happyfox001-noema/` 来源包，保留 README 快照、`github-api.json` 和 `metadata.json`
- 新增来源页 [[GitHub - Noema]]，并回写 [[Agent 框架设计]]、[[AI 工具化知识工作流]] 与 [[Agent 记忆与知识图谱]]
- Noema 先作为 voice-first desktop companion / 本地 agent runtime 样本保存；语音管线、桌面权限、插件权限、MCP manager、computer-use / browser-use 和 SQLite 记忆后续再隔离验证

- 整理用户新关注的 10 条 GitHub 仓库线索：全部可访问并迁入 `raw/repos/2026-06-09-github-*`，保留 README 快照、`github-api.json` 和 `metadata.json`
- 新增 10 篇来源页：[[GitHub - last30days-skill]]、[[GitHub - turbovec]]、[[GitHub - Google Skills]]、[[GitHub - Tolaria]]、[[GitHub - Agent Reach]]、[[GitHub - Personal AI Infrastructure]]、[[GitHub - Career-Ops]]、[[GitHub - PM Skills Marketplace]]、[[GitHub - whichllm]]、[[GitHub - claudesdk-skill]]
- 回写 [[AI coding framework]]、[[Agent 框架设计]]、[[AI 工具化知识工作流]]、[[Agent 记忆与知识图谱]]、[[提示词设计]] 与 [[机器学习工程入口]]
- 这批来源全部保持 `review`：多平台抓取、cookie / 认证、个人数据、求职自动化、benchmark、数据库/文件系统权限和 SDK skill 生成效果都待后续隔离验证
- 补出首批正式案例页：[[MyLLMWiki 分层知识库演化案例]]、[[Hive 音频数据集构造案例]]、[[Career-Ops 求职工作流工具化案例]]
- 补出首批领域页：[[AI Agent 与编程工作流]]、[[AI 工具化知识工作流]]、[[机器学习工程]]、[[信息聚合与调查]]、[[设计与产品系统]]
- 补出首批关系页：[[Prompt - 组织为 - Skill]]、[[数据监督纯度 - 影响 - 模型效果]]，并新增 [[案例索引]]、[[领域索引]]、[[关系索引]] 与相关控制面计数

## 2026-06-10

- 整理用户新关注的 6 条 GitHub 仓库线索：[[GitHub - turbovec]]、[[GitHub - Tolaria]]、[[GitHub - goose]]、[[GitHub - ChinaTextbook]] 已存在，未重复入库；其中 `block/goose` 已由现有 [[GitHub - goose]] 承接为 `aaif-goose/goose`
- 新增 1 个 repo 来源包和来源页：[[GitHub - system-prompts-and-models-of-ai-tools]]
- 将 `yikart/WeClone` 当前 Not Found 的仓库名保存为 seed：[[2026-06-10-yikart-weclone-待核实|yikart/WeClone 待核实]]
- 回写 [[提示词设计]]、[[AI coding framework]] 与 [[AI 工具化知识工作流]]；system prompt / internal tools 泄露类内容只作为安全边界样本保存，不迁出复刻或提取步骤

- 处理 `Clippings/` 新剪藏：Linux.do RAG 全流程实现教程（Java + 完整代码）
- 新增 `raw/web/2026-06-10-linuxdo-topic-2364008-rag-java-fullstack-tutorial/` 来源包：主帖正文与评论区切片（22-30 楼）合并保存，6 张内容图已本地化，emoji 表情图按论坛过滤规则保留远程链接
- 新增来源页 [[Linux.do - RAG 全流程实现教程（Java + 完整代码）]]，回写 [[Agent 记忆与知识图谱]]，并与 [[GitHub - Production Agentic RAG Course]] 建立跨技术栈 `互证` 关系
- 配套仓库 `worenbudaoni/rag-study-helper` 本轮未做 repo 快照，已登记到待处理 Review 区；来源页保持 `review`，教程参数不写成通用最佳实践

- 完成一次运行方式调整（经用户确认，结构与目录不变）：
- 清算 [[待处理]]：84 条 -> 9 条；75 条存量验证类事项按"工具跑测 / 交叉来源核实 / 合规边界复核 / 观察扩展候选"四类归档到新建的 [[验证债]]，按需取用、不要求清零；过期的 X 链接正文回填项放弃
- [[维护协议]] 新增两条规则：入库分级（新仓库 / 工具线索默认先登记进新建的 [[样本池]]，真正读过 / 用过 / 被论证需要时再升全套来源包和来源页）；验证缺口只写来源页 `当前边界`，不再自动生成待办
- `review` 状态重定义为"已存档、按需取用"的正常终态，写进 [[维护协议]] 来源页职责一节
- 按"被 2 个以上下游页面（主题 / 方法 / 概念 / 案例 / 对象 / 关系 / 领域页）实际引用"标准，把 65 篇来源页从 `review` 批量提为 `active`，并同步 [[来源索引]]；现 active 85 / review 41
- 存量 126 篇来源页不做回溯降级，原样保留

- 重写 [[首页]]（经用户确认）：从只增不减的"本轮补入"流水账改成回忆卡式入口——三种使用场景（投料 / 查询 / 行动）+ 结构一句话版 + 准确计数 + 当前活跃主线；历史流水账不再在首页重复记账，统一由本日志承载

- 处理 `Clippings/` 新剪藏：Linux.do Agent 岗位面试题实录（十几家公司）
- 新增 `raw/web/2026-06-10-linuxdo-topic-2365650-agent-job-interview-questions/` 来源包：主帖（约 200 道按公司分组的面试题，录音经 AI 整理）+ 评论区切片，无图片附件
- 新增来源页 [[Linux.do - Agent 岗位面试题实录（十几家公司）]]，回写 [[Agent 框架设计]]——这是该主题第一个需求侧（岗位市场在考什么）样本，与既有供给侧框架样本互补；并与 [[Linux.do - RAG 全流程实现教程（Java + 完整代码）]] 建立一供一需的补充关系
- 来源页保持 `review`：单一作者、单一时间窗、AI 转写可能失真，不外推为岗位市场全貌，不升面试准备方法页

- 修复：清理库根目录下 5 个 0 字节影子文件（案例索引 / 领域索引 / 关系索引 / 验证债 / 样本池，另有 1 个来源页影子）；真身均在 `_index/` 和 `wiki/sources/`，内容完好。成因是 Obsidian 在链接未解析时点击 wikilink 会按"新笔记默认位置 = 库根目录"创建空白同名笔记

## 2026-06-11

- 全量断链体检（起因：用户重启 Obsidian 后仍有多个链接点开是空白页）：扫描 296 个 md 文件
- 清理 2 个由误点未解析链接产生的根目录影子目录：`ohmybrew/`、`learn-anything/`（内含 0 字节文件）
- 修复 17 处断链：成因是历次维护轮在 [[待处理]]、[[验证债]]、运行日志里用"显示名"引用 seed 卡，而 seed 文件实际叫 `YYYY-MM-DD-slug` 格式，Obsidian 解析不到；已全部改写成 `[[实际文件名|显示名]]` 别名链接
- 复扫确认：全库断链 0
- 体检顺带发现 4 个 raw 层 README 抓取失败占位文件（rrweb / multica / presenton / bytebot，"README fetch failed: 403"），属来源包内容缺口而非断链，暂不处理
