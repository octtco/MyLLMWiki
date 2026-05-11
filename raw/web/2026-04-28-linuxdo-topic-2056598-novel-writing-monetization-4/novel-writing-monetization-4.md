---
title: "第四期赚钱技巧，deepseek有点牛逼（完整版本）"
source: "https://linux.do/t/topic/2056598"
author:
  - "[[user2609]]"
published:
created: 2026-04-28
description: "affb5dd85d863a999ef72430bdb40a2f1920×1200 272 KB 这个是我在cheery上，让他用得，加了一下提示词，第一次就弄到这个程度，有点牛逼啊，我看了一下，提示词就是我第三期发的那个110那个文档，等我去实际操作一下，我看一下最终效果怎么样"
tags:
  - "clippings"
---
[![affb5dd85d863a999ef72430bdb40a2f](https://cdn3.ldstatic.com/optimized/4X/5/4/7/547b1c91d3f85e8ab8c8d1839c130e6fd7b546b2_2_690x431.jpeg)

affb5dd85d863a999ef72430bdb40a2f1920×1200 272 KB

](https://cdn3.ldstatic.com/original/4X/5/4/7/547b1c91d3f85e8ab8c8d1839c130e6fd7b546b2.jpeg "affb5dd85d863a999ef72430bdb40a2f")

这个是我在cheery上，让他用得，加了一下提示词，第一次就弄到这个程度，有点牛逼啊，我看了一下，提示词就是我第三期发的那个110那个文档，等我去实际操作一下，我看一下最终效果怎么样？明天给各位反馈结果，就还是更新这个帖子，现在deepseek打折，我感觉可以得很

[![image](https://cdn3.ldstatic.com/optimized/4X/7/3/8/738a7deda8cfb558733f636f0993b59e173dfc74_2_335x500.png)

image722×1076 45.3 KB

](https://cdn3.ldstatic.com/original/4X/7/3/8/738a7deda8cfb558733f636f0993b59e173dfc74.png "image")

这章是用gemini生成得，但是改了好几次，才得到得，一样得提示词内容

实际测试效果，给各位佬汇报一下，非常抱歉，今天家里帮忙，现在才腾出时间。

deepseek是接入cc里面使用的，但是由于我本人不会用，现在用都是我朋友直接弄成现成的给我，怎么下载，然后怎么使用，连那个文件内容都是我朋友弄好给我的，除了那个cluade的skill.md指令是我让codex帮我生成的。

所以deepseek测试出来的结果有待改进，各位cc玩的好或者不是像我这样一样不同的小白，那效果应该更好

我先说一下我的操作，操作与第三期间没有区别，唯一区别，在于的是，多加了一步deepseek检查问题。

操作是这样的，由gemini cli生成一个初步大纲，这个大纲出来之后，我是丢进codex cli去检查的，然后找出问题来后，我是让他全部修正，给我生成一个完整具体的大纲，然后我把这个完整具体大纲又放到CC里面用deepseek去检查，我让他找出问题后，然后让他进行修正，修正后的大纲又放到codex cli里面去让他找i出问题

然后找出这个问题后，我把这些问题复制到cc里面，我是这样问的------这是由codex cli找出的问题，正确吗？

然后deepseek就会回答你问题，然后你让他全部修正，然后得出的大纲放到codex cli里面去，你问这个大纲怎么样？就这样一直循环，直到出现下面回答，那你可以直接丢到gemini cli里面去生成正文了

![屏幕截图 2026-04-26 230246](https://cdn3.ldstatic.com/original/4X/3/1/0/310e5b6bb84b4713a8d1f9626b27a4cf797a9d93.png)

[![屏幕截图 2026-04-26 230332](https://cdn3.ldstatic.com/original/4X/8/a/1/8a1ff4101f6e625875a3d0bf8e73fa17874b4c36.png)

屏幕截图 2026-04-26 2303321027×153 4.14 KB

](https://cdn3.ldstatic.com/original/4X/8/a/1/8a1ff4101f6e625875a3d0bf8e73fa17874b4c36.png "屏幕截图 2026-04-26 230332")

按照这个效果生成的大纲生成的效果图如下

gemini cli第一次生成

[![image](https://cdn3.ldstatic.com/optimized/4X/2/8/e/28e5a3c1a156444b7bdedc023f4cb43d9d19b119_2_690x459.png)

image1458×970 79.9 KB

](https://cdn3.ldstatic.com/original/4X/2/8/e/28e5a3c1a156444b7bdedc023f4cb43d9d19b119.png "image")

gemini cli根据指令优化后。指令是：查阅"C:\\Users\\31092\\Desktop\\JianQiDaMan\\57小说"里面的优秀小说，看一下人家在面对我们这样的港综场景、黑白切换、班底戏、商业起盘、堂口接盘时，人家的内容是怎么写得有人味、写得精彩，而不是看过去机械、AI味严重，然后把"写法机制"用在我们的内容上，优化我们的正文，给我优化后的小说正文！

[![image](https://cdn3.ldstatic.com/optimized/4X/d/3/e/d3e98ffc2080afca547e050802e3637ee59b529a_2_688x500.png)

image1376×1000 64.8 KB

](https://cdn3.ldstatic.com/original/4X/d/3/e/d3e98ffc2080afca547e050802e3637ee59b529a.png "image")

deepseek第一次生成

[![image](https://cdn3.ldstatic.com/optimized/4X/c/7/7/c77dde3f09d0f3479e8375dd441a7a16023da495_2_548x499.png)

image1064×970 55.4 KB

](https://cdn3.ldstatic.com/original/4X/c/7/7/c77dde3f09d0f3479e8375dd441a7a16023da495.png "image")

deepseek根据指令优化后的内容，和上面指令是一样的

[![image](https://cdn3.ldstatic.com/optimized/4X/6/1/a/61ab10e2d1e0498f62e9a9e26885989609378c59_2_381x500.png)

image1010×1324 75.4 KB

](https://cdn3.ldstatic.com/original/4X/6/1/a/61ab10e2d1e0498f62e9a9e26885989609378c59.png "image")

下面这个是我把四个生成的内容，就是里面写的好的内容，看着更像人写的内容进行的替换，替换顺序是这样的，以gemini cli第一次生成的内容为蓝本，先把gemini cli2次优化后的内容进行挑选，

然后再根据deepseek生成的内容进行一个挑选，这一步可以要，也可以不要，只要你觉得在gemini cli那两次融合后的ai率让你满意，那就不用麻烦了

接着就是，把你满意后的内容又放在gemini网页端去生成，也是找内容来进行代替，这一步也是，可有可无，如果你对你的ai率满意

不要觉得后面生成的ai率比1第一次生成的还高，就觉得优化没有作用，有作用的

这个第一张照片是由gemini cli第一次内容为蓝本，然后根据gemini cli优化的内容进行了替换以及我自己删除了一些多余的内容出现的结果

[![image](https://cdn3.ldstatic.com/optimized/4X/4/c/b/4cbdcaa90ab9913b2f5d325311f08b5264acb329_2_401x500.png)

image902×1122 57.5 KB

](https://cdn3.ldstatic.com/original/4X/4/c/b/4cbdcaa90ab9913b2f5d325311f08b5264acb329.png "image")

这个第2张照片，则是由上面第一张照片检测的内容再根据deepseek生成的内容继续进行替换内容得到的，

[![image](https://cdn3.ldstatic.com/optimized/4X/f/e/2/fe2b9a3732658ef9b61813bffd066ebc39df0e6f_2_343x500.png)

image756×1102 48.3 KB

](https://cdn3.ldstatic.com/original/4X/f/e/2/fe2b9a3732658ef9b61813bffd066ebc39df0e6f.png "image")

这张图片做一个声明，标红的内容是最后几排的内容，但是我认为是不应该标红的，这撒比朱雀有问题

请看对比：这是标红的内容：“没拿钱的苦力要吃饭，让他们闹。”

这是没有标红的内容："不拦第一步，拦第二步。"这句话不是一眼ai吗？朱雀居然只是把他标注为疑似ai，我真的服了

“第一，合法的劳资讨薪，我们不动。”

最后，我发现了朱雀的检测盲点，他是真有问题，我只是在刚刚那个标红的内容删除了一些词语：在安静的顶层套房里显得干涩而冷硬；发出有节奏的哒哒声；“让律师同步到场，与领事馆防务联络线互留书面时间戳。”，这样ai率就标绿了，我只能说一个大写的6

[![屏幕截图 2026-04-27 020128](https://cdn3.ldstatic.com/optimized/4X/7/e/2/7e26a48daf549000afac7248fe26cc8d2a9c3e9c_2_341x499.png)

屏幕截图 2026-04-27 020128757×1108 48.4 KB

](https://cdn3.ldstatic.com/original/4X/7/e/2/7e26a48daf549000afac7248fe26cc8d2a9c3e9c.png "屏幕截图 2026-04-27 020128")