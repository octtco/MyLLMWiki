# 运行日志

这里记录比较重要的 ingest、compile、query、回写和修补动作。

建议每次只记短条目，重点放在“做了什么”和“下一步是什么”。

## 2026-04-13

- 初始化知识库骨架
- 补充维护协议、索引页、模板
- 增加 `raw` 来源包约定
- 增加健康检查页和输出状态约定

## 2026-04-14

- 把 `raw/web/Clippings/即梦真无限sd2.0无限画图视频教程！不是标题党！超级简单 - 福利羊毛  福利羊毛, Lv1.md` 编译为首篇来源页
- 更新来源索引和总览计数
- 在待处理队列里加入“补交叉来源验证”和“后续可抽象页面”两项
- 基于 GitHub 仓库主页与 linux.do 推广帖，为 GenericAgent 新增两篇来源页
- 在待处理队列里加入“README 可回证主张 vs 帖子宣传口径”的复查项

- 将 `raw/web/羊毛/即梦真无限sd2.0无限画图视频教程！不是标题党！超级简单 - 福利羊毛  福利羊毛, Lv1.md` 规范化为标准来源包 `raw/web/2026-04-14-linuxdo-topic-1956835-jimeng-unlimited/`
- 下载 1 张远程图片到来源包本地 `images/` 并将正文主文件中的图片链接改为相对路径
- 修正即梦来源页的 `source_path`、`source_bundle` 和回链，使其重新对齐已规范化的 raw bundle
- 将 GenericAgent 的 linux.do 帖子规范化为标准来源包 `raw/web/2026-04-14-linuxdo-topic-1962519-genericagent-self-evolving-agent/`
- 为 GenericAgent 的 GitHub README 建立本地 repo 来源包 `raw/repos/2026-04-14-github-lsdefine-genericagent/`
- 更新首页、待处理和健康检查，让运行面和当前仓库状态重新对齐
- 将 Trellis 的 linux.do 帖子规范化为标准来源包 `raw/web/2026-04-14-linuxdo-topic-1539636-trellis-best-practice/`
- 为 Trellis 的 GitHub README 建立本地 repo 来源包 `raw/repos/2026-04-14-github-mindfold-ai-trellis/`
- 新增 Trellis 的 GitHub 主来源页与 linux.do 设计动机来源页
- 更新来源索引、待处理、总览，让 Trellis 进入正式维护流程
- 为 GenericAgent 与 Trellis 的帖子执行远程图片本地化，成功保留主体配图，少量头像与 emoji 因源站限制保留原链接
- 在 4 篇来源页里补充“可回证能力/主张”与“经验判断/宣传口径”拆分
- 新增概念页 `自进化 Agent`，并把 Trellis 和 GenericAgent 的来源开始接入知识网络
- 同步更新概念索引、待处理、总览和健康检查

## 2026-04-15

- 将根目录 `Clippings/【教程】6.5 块 Plus 与 2.5 块 Team 的获取渠道 - 福利羊毛  福利羊毛, Lv1.md` 迁移为标准来源包 `raw/web/2026-04-15-linuxdo-topic-1969970-plus-team-channels/`
- 为该来源新增来源页 `Linux.do - 6.5 块 Plus 与 2.5 块 Team 的获取渠道`
- 尝试执行远程图片本地化，但图片源站超时或 TLS 中断，保留原链接并把失败记录写入 metadata
- 更新来源索引、待处理、总览和健康检查，并将已处理原文件从 `Clippings/` 收件箱移除
- 从这篇来源里进一步抽出概念页 `顺藤摸瓜式搜索`，把“找渠道”上提为更通用的搜索方法
- 为 GenericAgent 和 Trellis 这两组双来源样本补第一批保守关系，显式区分 `定义`、`支持`、`宣传`、`补充` 和 `主说明`
- 新增主题页 `Agent 框架设计`、`AI coding framework`，把已有 concept/source 关系接到主题层
- 更新来源索引、概念索引、主题索引和待处理队列，使关系层与主题层开始同步进入运行态
- 将原先混在一起的 Spec/Skill 复合表达拆回两个原子概念 `Spec`、`Skill`，并把相关内容降成关系/主题层表达
- 统一把 `raw/web/` 与 `raw/repos/` 的文本主文件改成与来源包同名的唯一 `.md` 文件，避免图谱里出现大量同名节点
- 更新来源页回链、维护协议、skill 规范和健康检查口径，让“原子概念 + 唯一来源主文件”成为当前默认规则
- 将来源包里的文本主文件进一步收缩成简短直观的语义名，如 `trellis.md`、`genericagent.md`、`plus-team-channels.md`，并保留按需最小消歧的规则
- 为 `Lucent-Snow/anti-default-output` 新建标准 repo 来源包，并补充 README、`SKILL.md` 与分场景 reference 快照
- 新增来源页 `GitHub - anti-default-output` 与概念页 `反默认输出`，把“识别默认路径后主动偏离”的方法接入知识网络
- 更新 `Skill` 概念页、来源索引、概念索引、待处理和总览，使“纠偏型 skill” 进入当前知识库结构

## 2026-04-16

- 围绕 `anti-default-output` 继续细化概念层，把原先塞在 `反默认输出` 里的隐含方法拆成 `默认路径` 与 `输出前自检` 两个原子概念
- 扩写 `GitHub - anti-default-output` 与 `反默认输出`，显式写出”识别对象 -> 前置检查 -> 执行偏离”的方法链路
- 更新 `Skill`、来源索引、概念索引和总览，让”纠偏型 skill 不只给方向，也封装判断动作”这层结构在图谱里可见
- 执行知识库整理：检查 `Clippings/` 收件箱（已空）、健康检查项、待处理队列
- 尝试本地化 `plus-team-channels.md` 中的远程图片，但源站连接超时，保留原链接
- 确认孤立来源页 `Linux.do - 即梦真无限sd2.0无限画图视频教程` 已标注相关概念和主题，但这些概念/主题页暂不创建（证据不足）
- 当前状态：`Clippings/` 已清空，7 个来源页，7 个概念页，0 个关系页，2 个主题页

## 2026-04-17

- 将根目录 `Clippings/面向过程 VS 面向对象.md` 迁移为标准来源包 `raw/web/2026-04-16-zhihu-procedural-vs-object-oriented/`
- 成功本地化 3 张正文配图，并把主文件中的远程图片改写为来源包内相对路径
- 新增来源页 `知乎专栏 - 面向过程 VS 面向对象`，并将其接入概念页 `面向过程`、`面向对象`
- 新增概念页 `面向过程` 与 `面向对象`，把这篇知乎入门材料正式接入知识网络
- 更新概念索引、待处理、健康检查、总览和首页；移除这篇来源的孤立来源标记，但仍暂不新建“编程范式”主题页

## 2026-04-20

- 为《工程控制论》（第三版）建立标准来源包 `raw/books/2026-04-20-qianxuesen-engineering-cybernetics-3e/`，并把上下册 PDF 复制到 `files/` 中做原始层留存
- 新增来源页 [[工程控制论（第三版）]]，把这本书正式接入 `wiki/sources/`
- 新增主题页 [[控制论式系统思维]]，把“先建模、再分析、再设计、再处理不确定性”的方法主线沉淀到 `wiki/topics/`
- 给输出页《工程控制论-读前导览》和《工程控制论-通用方法提炼：用于项目、学习与组织》补了“依据与判断边界”，显式区分原书直接支持与维护者迁移判断
- 更新来源索引、主题索引、待处理、总览计数，并在 raw 层文档中补入 `books/` 目录约定

## 2026-04-21

- 在 `outputs/reports/2026-04-21-工程控制论-融合版/` 下新增 1-2 章融合版工作页：保留旧结构版的拆解骨架，同时全部改用 PDF 正文页码做支撑
- 新增 `00-融合说明.md`，明确区分“直接支持”和“低强度归纳”，把这一轮试跑的比较标准写清
