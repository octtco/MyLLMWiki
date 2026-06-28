---
title: "【开源自荐】Marginalia：一个面向私人异构资料库的 AI 检索 / 调查系统"
source: "https://linux.do/t/topic/2264632"
author:
  - "[[MinQ]]"
published:
created: 2026-06-19
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

[![marginalia-promo](https://cdn3.ldstatic.com/optimized/4X/5/6/e/56e94563b26a5cc6285c42995f03aaf2d59e4b57_2_690x388.jpeg)

marginalia-promo1672×941 253 KB

](https://cdn3.ldstatic.com/original/4X/5/6/e/56e94563b26a5cc6285c42995f03aaf2d59e4b57.jpeg "marginalia-promo")

  

[![desktop-screenshot-zh-CN](https://cdn3.ldstatic.com/optimized/4X/1/4/4/144eb37c652946072594aa73ec77c155d158fc43_2_660x500.jpeg)

desktop-screenshot-zh-CN2202×1668 304 KB

](https://cdn3.ldstatic.com/original/4X/1/4/4/144eb37c652946072594aa73ec77c155d158fc43.jpeg "desktop-screenshot-zh-CN")

最近被老板按着头做知识库做的心烦，白天向量数据库晚上切块的，效果还越调越烂，日子过得贼难受  
这不得不促使我思考一个问题，人类管理书籍和档案已经几千年了，也没听说过有向量数据库这玩意啊，那不也活得好好的  
然后我也研究了一些比如最近大火的Karpathy LLM Wiki之类的，但感觉都差点意思，不太适合企业级（至少是中小企业起步吧）知识库的做法。

想来想去，我决定拿出毕生所学，捣鼓了一个（自我感觉）非常适合研究者/法律工作者/金融工作者这个方向的知识库

它的底层逻辑就是  
图书馆学 x 推荐系统 x Agent

整个系统以不同角色为边界，划分了3个角色：图书馆员，调查员，用户  
用户负责上传文件，图书馆员负责对文件打标签，写summary。调查员负责写笔记、阅读summary，浏览不同的文件提取知识，并最终汇总成调查报告发给用户，同时记下这次问答的笔记。图书馆员再利用这个笔记将不同的文件进行聚合，挖掘不同文件之间的内在关联，这样一个知识图谱就形成了

而且整个系统是一个自反馈系统，随着问的问题越来越多，它就能够挖掘出你在跟它对话中隐藏的知识关联性和文件隐含的其它属性，提高聚合和查询的质量

最终的目标是诞生一个自组织、自适应、自感知的知识库系统

目前已经有几个种子用户，他们一致认为该项目能够解决工作中的很多问题

Github: [GitHub - shenmintao/marginalia: A library-science-inspired personal knowledge management system with LLM agents · GitHub](https://github.com/shenmintao/marginalia)

希望大家多多体验，提点反馈意见

目前的评测方法是加载了一些公开的法律相关文件，然后对公开判决进行审查，给出理由和反对意见，然后抓一个正经法官过来进行评测，结论是大约跟法官助理水平相当。

---

## Comments

> **hwang** · [2026-05-28](https://linux.do/t/topic/2264632/3?u=lelele1)
> 
> 用户上传文件后，图书馆员Agent 把文件按分类、标签放到了各自的位置（模拟），然后有需要的时候找调查员Agent 去根据文件的分类、标签、元数据等，再结合知识图谱（记忆）去找对应的文件出来？  
> 优点是可以很快得找到对应的文件，缺点是没法通过细节、内容去找，然后这个缺点依赖使用的过程中不断演化完善的知识图谱去弥补，我的理解对吗？