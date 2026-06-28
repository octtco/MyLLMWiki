---
title: "Bili Note：把 B 站视频和图文整理成可追问的 Markdown 笔记"
source: "https://linux.do/t/topic/2452065/2"
author:
  - "[[chuanbai]]"
published: 2026-05-23
created: 2026-06-22
description: "本帖使用社区开源推广，符合推广要求。我申明并遵循社区要求的以下内容： 我的帖子已经打上 开源推广 标签： 是 我的开源项目完整开源，无未开源部分： 是 我的开源项目已链接认可 LINUX DO 社区： 是 我帖子内的项目介绍，AI生成、润色内容部分已截图发出： 是 以上选择我承"
tags:
  - "clippings"
---
#### 本帖使用社区开源推广，符合推广要求。我申明并遵循社区要求的以下内容：

- **我的帖子已经打上 [开源推广](https://linux.do/tag/2234-tag/2234) 标签：** 是
- **我的开源项目完整开源，无未开源部分：** 是
- **我的开源项目已链接认可 LINUX DO 社区：** 是
- **我帖子内的项目介绍，AI生成、润色内容部分已截图发出：** 是
- **以上选择我承诺是永久有效的，接受社区和佬友监督：** 是

*以下为项目介绍正文内容，AI生成、润色内容已使用截图方式发出*

---

# Bili Note：把 B 站视频/图文整理成可追问的 Markdown 笔记

各位佬友好，分享一个我最近做的小工具：Bili Note。

项目地址：

[github.com](https://github.com/Rimagination/bili-note)

![](https://cdn3.ldstatic.com/optimized/4X/9/7/7/9774117ba8e44d04fcddeb902c044c7134de7504_2_690x344.png)

### [GitHub - Rimagination/bili-note: Extract Bilibili videos into learning-oriented...](https://github.com/Rimagination/bili-note)

Extract Bilibili videos into learning-oriented Markdown notes with full subtitle and comment archives

它是一个给 Codex / Agent 用的 skill，主要用途是把 B 站视频、图文、动态/opus 内容整理成本地 Markdown 笔记，并且把完整字幕、图文正文、图片、评论、元数据和证据索引一起归档。

我做它的原因很简单：很多 B 站技术视频、课程视频、观点视频，其实不是“总结一下”就够了。

真正有用的是：

1. 能保留完整原始材料，后面可以继续追问；
2. 不把 5 分钟视频和 70 分钟课程都压成差不多长；
3. 根据视频时长、字幕量、收藏、点赞、评论、弹幕、发布时间等信号，动态决定笔记该写多细；
4. 关键判断能用 `[1][2]` 这种论文式编号链接回原文证据。

所以 Bili Note 的目标不是生成几句摘要，而是生成一份适合学习、复习、放进 Obsidian，并且后续还能让 Agent 继续问答的知识库材料。

## 它能做什么

- 提取 B 站视频内容，生成学习型 Markdown 笔记
- 提取 B 站图文 / opus / 动态长文
- 可选提取评论区里有用的技术讨论
- 保存完整字幕、正文、图片、评论和元数据
- 生成证据索引，方便回查原文
- 根据内容信息量和互动质量控制笔记长度
- 支持保存到指定文件夹或 Obsidian 知识库

## 使用方式

在 Codex 里安装：

```plaintext
请帮我安装这个 skill：
https://github.com/Rimagination/bili-note
```

提取一个视频：

```plaintext
请帮我提取这个视频的内容：https://www.bilibili.com/video/BVxxxx/
```

如果要保存到自己的知识库：

```plaintext
帮我存放在：“D:\知识库\B站总结” 里
```

如果要连评论区一起整理：

```plaintext
请帮我提取这个视频的内容和评论区有用的内容：https://www.bilibili.com/video/BVxxxx/
```

图文也可以：

```plaintext
请帮我提取这个 B 站图文的内容：https://www.bilibili.com/opus/xxxx
```

## 一个比较重要的设计

Bili Note 不是固定长度总结器。

它会先根据原始材料生成一个“笔记预算”，比如视频多长、字幕多少字、证据块多少、互动质量如何，然后再决定笔记大概应该写多少字。

这样长课程不会被压成短摘要，短视频也不会被硬扩写成大论文。

## 依赖和限制

默认路线主要依赖 B 站公开接口，可以抓元数据、公开字幕、图文、评论等。

如果视频没有公开字幕，增强路线可以尝试通过 Chrome + web-access 获取网页 AI 字幕。  
如果还是没有字幕，也可以走本地 ASR 转写，但这部分需要 ffmpeg 和 Whisper / faster-whisper / FunASR 之类的后端。

也就是说：核心功能尽量轻依赖，字幕兜底能力按需增强。

## 适合谁

如果你经常在 B 站看 AI、编程、科研、工具教程，并且希望把视频沉淀到自己的知识库里，这个 skill 应该会比较有用。

欢迎佬友试用、提 issue，也欢迎直接改。

这个项目做完发出来还挺火的，应该是有很多人有需求，我就想到在Linux Do也发一下：  

[![image](https://cdn3.ldstatic.com/optimized/4X/3/5/0/350a2d5f1faa0145c153d119c242efcc5e9d2de0_2_690x471.png)

image1783×1218 177 KB

](https://cdn3.ldstatic.com/original/4X/3/5/0/350a2d5f1faa0145c153d119c242efcc5e9d2de0.png "image")

最后，附上 AI 润色截图：  

[![image](https://cdn3.ldstatic.com/optimized/4X/3/5/0/350a2d5f1faa0145c153d119c242efcc5e9d2de0_2_690x471.png)

image1783×1218 177 KB

](https://cdn3.ldstatic.com/original/4X/3/5/0/350a2d5f1faa0145c153d119c242efcc5e9d2de0.png "image")

---

## Comments

> **Anya\_Forger** · [2026-06-22](https://linux.do/t/topic/2452065/2?u=lelele1)
> 
> 不错诶 最近就在b站上学习 这个项目很好 已star

> **xuyanz** · [2026-06-22](https://linux.do/t/topic/2452065/3?u=lelele1)
> 
> 好东西啊 感谢佬开源 之前我一般是批量下载字幕 建立本地知识库  
> 太耗费时间了

> **MYFriend** · [2026-06-22](https://linux.do/t/topic/2452065/4?u=lelele1)
> 
> 好东西，之前就想弄个提取b站字幕的，那些内置字幕的视频能提取字幕吗？