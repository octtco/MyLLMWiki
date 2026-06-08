# 健康检查

这页记录当前知识库的结构健康状况。

## 当前结论

- 仓库控制面已对齐到最新版结构口径：`source / entity / topic / method / concept / case / domain / relation + goal / task`
- 《工程控制论》这条长材料链已经补齐 `outputs` 工作层，并正式回写到来源页、主题页、10 篇方法页和 20 个相关概念页
- 当前没有明显的结构性欠账，健康检查未修项可暂记为 0
- 当前计数继续只算正式页面，不计 `README.md`、`.gitkeep` 这类占位文件

## 已确认正常

- 首页、总览、维护协议、README、对象索引、目标索引和方法索引已经统一到同一版结构口径
- 当前计数已经重新对齐：113 个来源页、5 个正式对象页、1 个正式目标页、18 个主题页、14 个方法页、29 个概念页、23 个输出页、70 个待处理项
- 来源页都已经重新接回索引
- `wiki/methods/` 不再是空目录，当前已有 14 篇正式方法页
- 《工程控制论》相关的来源页、主题页、方法页、概念页之间已经接回显式链接
- `outputs/` 里已经有对应的长文工作层，且 `00-07` 已经形成完整工作链，不再直接从整本书跳到正式页
- `系统类型`、`非线性系统`、`信息`、`大系统` 等候选继续留在宿主页或工作层，是刻意的筛页结果，不算结构欠账
- 规程类 `reports` 继续留在 `outputs/`，符合“先做样板，再决定是否 promote”的当前策略
- 高风险论坛帖目前仍停留在保守表达，没有被写成强结论
- `seeds/inbox/` 这一轮已经成功分流出 4 张能升正式来源的卡，只把 `Grok 镜像站` 留作高波动入口线索
- `raw/chats/` 已经不再只是 README，现在既有批次级总归档，也有 `MyLLMWiki`、`WeBox`、`WhatsBox`、`Beam` 这四份项目级切片样板
- `Clippings/` 这轮又成功分流出一组 7 篇 Linux.do 小说写作系列来源，并正式接成 7 篇来源页、1 个主题页和 3 条方法页
- `Clippings/` 里的不完整论坛评论截片现在也会改走 `seeds/`，不再为了清空收件箱硬补成弱来源页
- `Clippings/` 这轮又成功分流出 3 篇新网页剪藏，并按保守口径补成 3 篇 `review` 来源页
- `MyLLMWiki` 已经有了第一篇正式对象页和第一篇正式目标页，对象层和目标层不再只是模板
- skill 与 reference 里的路由口径已经同步到“统一收件箱 -> raw / seeds / todo / wiki / outputs”这条新版主路径
- 上轮写进 [[AI coding framework]] 和 [[Agent 框架设计]] 的 `Codex / Gemini / WebBridge / TRINITY / AutoScientist` 线索，这轮已经补成正式来源页，不再只停在 topic 正文里的外部链接
- [[把 MyLLMWiki 跑成可持续增长的个人 LLM Wiki]] 已经通过 [[2026-05-20-当前知识库适配-Karpathy-LLM-Wiki-盘点]] 完成阶段性收口；Karpathy 适配不再是开放待办
- `Clippings/` 当前只剩 README / `.DS_Store` 这类非资料文件；重复 Hive PDF 已核对移除，两篇 2026-05-20 Linux.do 剪藏已迁入 `raw/web/` 并补来源页
- `raw/web/2026-05-19-*` 这一组最小快照已经补齐 `metadata.json`，不再是缺元数据来源包
- 2026-05-28 这一轮新增 6 个 GitHub repo 来源包，均保留 README 快照和 GitHub API 原始响应；ChinaTextbook 已按许可待审边界保守保存
- 2026-05-29 这一轮新增 4 个 GitHub repo 来源包，均保留 README 快照和 GitHub API 原始响应；developer-roadmap 已记录原请求名与 canonical 仓库名差异
- 2026-06-01 这一轮新增 8 个 GitHub repo 来源包，均保留 README 快照和 GitHub API 原始响应；`rsshub` 和 `javascript-algorithms` 已按 GitHub 搜索第一结果映射到 canonical 仓库
- 2026-06-02 这一轮新增 4 个 GitHub repo 来源包，均保留 README 快照和 GitHub API 原始响应；[[GitHub - Scrapling]] 已存在，未重复入库
- 2026-06-03 这一轮新增 5 个 GitHub repo 来源包，均保留 README 快照和 GitHub API 原始响应；[[GitHub - Supermemory]] 已存在，未重复入库
- 2026-06-04 这一轮新增 1 个 GitHub repo 来源包，保留 README 快照和 GitHub API 原始响应
- 2026-06-05 这一轮新增 2 个 GitHub repo 来源包，均保留 README 快照和 GitHub API 原始响应
- 2026-06-08 这一轮新增 10 个 GitHub repo 来源包，均保留 README 快照和 GitHub API 原始响应；另有 7 个 GitHub API 返回 Not Found 的仓库名保存为 seed 待核实

## 需持续观察

- 《工程控制论》这一组方法和概念目前仍主要由单一来源支撑，跨到项目、学习、组织场景时仍应保持低强度表述
- `逻辑控制`、`有限自动机`、`信息`、`大系统` 这些更大的后段线索，后续若要升更高层页面，最好等更多来源一起补进来
- `AI coding framework` 和 `Agent 框架设计` 这两页目前仍主要由项目方来源与论坛帖支撑，后续要靠更多外部样本来稳
- `反默认输出`、`默认路径`、`输出前自检` 这组三页目前仍以单一 repo 为主来源，暂不宜继续上提成更大主题
- `Malus.sh - 官方落地页` 目前只有官网自述口径，法律和版权边界仍要靠更多独立来源来定
- `404 Media - 官方介绍` 与 `Futurism - 首页定位快照` 目前更像媒体入口记录；是否升对象页，最好等它们在更多来源里反复出现之后再说
- `Codex rollout 历史聊天归档（2026-02 至 2026-04）` 现在已经有了 `MyLLMWiki`、`WeBox`、`WhatsBox`、`Beam` 这四份项目级切片；但当前明确继续跟进的先只留前三条，`Beam` 先留档不扩
- `Somnus` 当前虽然也有 7 个 session，但其中夹着多条打招呼和跑偏会话；在它继续积累出更实的工程语境前，先不急着升对象页
- `AI 辅助网文写作` 这组新来源目前仍主要是单作者系列经验帖；平台热度、AI 检测器和具体模型搭配都应继续保守处理
- 新收进来的两篇 GoPay / GPT Plus 来源当前都只适合保留为高时效支付路径样本；GoPay 注册、1 印尼盾试用、退款回流、直跳 checkout 脚本和“无需印尼节点”这些说法都还不能写成稳定机制
- 新收进来的 [[Linux.do - Seedance 2.0 结合 GPT 的导演思维教学]] 当前能稳住的主要是“先把粗剧情改写成镜头级分镜，再喂给模型”这条前置流程；更多私下资料和效果迁移性都还待验证
- 新收进来的 [[Linux.do - 自建家宽节点与中转站部署教程]] 混着通用 VPS 运维、家宽中转链路和高风险用途判断，当前更适合保留为部署样本，不适合直接抽正式方法
- 新收进来的 [[Linux.do - 学生创业的 10 道坎]] 目前仍是单一作者的强观点复盘；哪些是共性结构问题、哪些只是叙事放大，还需要更多独立来源来稳
- `seeds/inbox/` 现在除了旧的高波动入口线索，还新增了 `实时多模态交互`、`多模态生成能力簇`、`麻醉语言预测与 AI 类比` 这 3 张待分流卡；当前继续保留为 seed 是刻意保守，不算结构欠账
- 这组来源里挂着的 txt / zip 附件这轮还没有本地化，当前仍主要靠原始外链回证
- [[Linux.do - GPT Image 2.0 生图 50 种风格速查表]] 里的两张展示图仍是远程 Linux.do 图片，本轮只保留原始链接，未做本地化
- [[GitHub - ChinaTextbook]] 的教材版权 / 许可边界仍需单独复核；当前不下载 PDF，不把它升成稳定学习资源主题
- [[GitHub - MarkItDown]]、[[GitHub - Sim]]、[[GitHub - Open Deep Research]] 和 [[GitHub - MindsDB]] 当前只按 README 整理，后续若要作为工具推荐应先做真实任务跑测
- [[GitHub - Graphiti]] 当前只按 README 整理，后续若要作为 agent memory 推荐，应补最小试用和 GraphRAG / RAG 对照
- [[GitHub - Hyperswitch]] 当前只保留为支付基础设施来源页，支付合规和生产接入边界仍需独立资料支撑
- [[GitHub - AI Hedge Fund]] 当前仅作为教育研究样本保存，不提供投资建议，后续需补金融合规和回测方法边界
- [[GitHub - TradingAgents]] 当前仅作为多 agent 金融研究框架样本保存，不提供投资建议，后续需补金融合规、数据来源和回测方法边界
- [[GitHub - MoneyPrinterTurbo]] 当前只作为短视频自动化工具样本保存，素材版权、平台规则和批量生成边界仍需复核
- [[GitHub - Scrapling]] 当前只作为网页采集框架样本保存，不扩写反爬或绕限制步骤
- [[GitHub - Flowsint]] 当前只作为 OSINT 图谱调查工具样本保存，不扩写个人画像、泄露库查询或目标侦察步骤
- [[GitHub - VoxCPM]] 当前只作为语音生成 / 声音克隆模型样本保存，声音授权、身份安全和合成内容标注仍需复核
- [[GitHub - Machine Learning for Trading]] 当前只作为金融机器学习学习样本保存，不提供投资建议，依赖和数据源仍需复核
- [[GitHub - Production Agentic RAG Course]] 当前只作为生产级 RAG 课程项目样本保存，未跑通服务链路
- [[GitHub - Aegis]] 当前只作为 AI coding agent method-pack / workflow discipline 样本保存，未验证多 host 安装和现有规则叠加
- [[GitHub - gstack]] 当前只作为 AI coding agent 角色化 skill stack 样本保存，未验证 setup、team mode、浏览器、iOS QA、deploy、安全审计和多 host 行为
- [[GitHub - fishkeeper]] 当前只作为闲鱼 / 闲管家开放平台的垂直业务 API skill 样本保存，未验证官方授权、真实店铺 API 调用、订单操作和凭据安全
- [[GitHub - Vanna]] 与 [[GitHub - MCP Toolbox for Databases]] 当前只作为数据库 AI / MCP 工具样本保存，未验证只读权限、审计、鉴权和真实数据库风险
- [[GitHub - AIHawk]] 当前只作为求职自动化高风险样本保存，仓库已 archived，不迁出自动投递步骤
- [[GitHub - kanata]]、[[GitHub - node-clinic]]、[[GitHub - PraisonAI]]、[[GitHub - open-notebook]]、[[GitHub - goose]] 和 [[GitHub - whisper.cpp]] 均未做本地安装或最小运行验证
