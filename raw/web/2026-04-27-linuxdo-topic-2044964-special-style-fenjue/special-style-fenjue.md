---
title: "通用焚决千篇一律，特殊风格万里挑一 | 一些非大流二次元向自用Prompt合集 | 一些自制焚决的思路"
source: "https://linux.do/t/topic/2044964/2"
author:
  - "[[sallyn]]"
published: 2026-04-27
created: 2026-04-27
description: "写在前面 GPT-Image-2 也出了有一段时间了。从一开始制作各种IP的联动图，到使用各路大神写的焚决，也算是把这个模型的能力体验的七七八八了。 但是同样的主题和同样的焚决看多了，加上大家用的都是一个模型，所以很多时候看到一张图，就会想“哦这是GPT做的 真好看啊”然后就忘了"
tags:
  - "clippings"
---
## 写在前面

GPT-Image-2 也出了有一段时间了。从一开始制作各种IP的联动图，到使用各路大神写的焚决，也算是把这个模型的能力体验的七七八八了。

但是同样的主题和同样的焚决看多了，加上大家用的都是一个模型，所以很多时候看到一张图，就会想“哦这是GPT做的 真好看啊”然后就忘了。

其实这个道理和前端也是一样的，如果让我回到过去一两年前，看到AI能做出一个还可以的蓝紫渐变网站那会，我可能会觉得还不错——但是时间长了千篇一律的设计风格看多了难免有些乏味。现在的 GPT-5.4 在这上面的缺陷就很大——衬线体大字hero标题、卡片堆砌、无意义的说明文字。如果是乍看一眼我会觉得还行，但看多了确实没意思。

因此在用了各种焚决之后，我打算从 Pinterest 以及 X 上的各种插画参考，自己写不曾在 GPT-Image-2 中看过的设计风格。

## 先来几个例子

> 这是一个很通用的GPT风格，仅作对比。

### 电商联动宣传物料

```markdown
生成一张 偶像大师闪耀色彩 樱木真乃 联动奶茶品牌 喜茶 的活动宣传图。竖屏比例。人物占据画面右侧三分之二的空间，左侧为喜茶品牌logo和新品名字“春日雪乃”，下接活动宣传语，以及相关杯型的价格。还有小字注明奶茶用料包含什么成分。文艺风格。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![image](https://cdn3.ldstatic.com/optimized/4X/c/1/6/c1657d6baeb348bda06ce362e524d8ac7b4bc2ec_2_333x500.jpeg)  image853×1280 205 KB  ](https://cdn3.ldstatic.com/original/4X/c/1/6/c1657d6baeb348bda06ce362e524d8ac7b4bc2ec.jpeg "image") | [![image](https://cdn3.ldstatic.com/optimized/4X/d/8/d/d8d63d6057fa98db7b585e0ef30687493f789a4b_2_333x500.jpeg)  image1024×1536 378 KB  ](https://cdn3.ldstatic.com/original/4X/d/8/d/d8d63d6057fa98db7b585e0ef30687493f789a4b.jpeg "image") |

这个我自己在小红书上发的大概是有9w阅读，6k赞 + 3k 收藏，所以大概这个风格已经在各个地方都能看到了。其实提示词对风格的限制很少，基本依赖于模型本身自行发挥的能力，~~因此现在看到联动图我已经有点麻木了~~。

![image](https://cdn3.ldstatic.com/original/4X/5/f/f/5ff70e7fa87d0b89a23a905452f812d9cbb92b13.png)

> 那么就让我们来做点不一样的风格吧

### 俄国解构主义

```markdown
生成一张 deepseek v4 的宣传海报，要求将 deepseek v4 拟人化成一个动漫女性角色。俄国构成主义风格，平面设计插画，极简主义矢量艺术，复古宣传海报。画面由强烈的几何形状构成，包含大量的锐利三角形、圆形和粗重的对角线切割。色调采用极简的三色限定：高饱和度宝蓝色、深黑色和米白色（做旧纸张感）。整体具有复古丝网印刷质感，布满细腻的颗粒噪点和磨损纹理。构图充满张力，强调不对称的平衡感和工业力量感，锐利的线条边缘，扁平化视觉，高对比度。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![image](https://cdn3.ldstatic.com/optimized/4X/0/d/6/0d6848cf42a024c4f6522bc1dee9e7a05c9c4a4e_2_375x500.jpeg)  image960×1280 514 KB  ](https://cdn3.ldstatic.com/original/4X/0/d/6/0d6848cf42a024c4f6522bc1dee9e7a05c9c4a4e.jpeg "image") | [![image](https://cdn3.ldstatic.com/optimized/4X/0/7/5/0754a494bf39c9e82b35816243492408e3860582_2_375x500.jpeg)  image1086×1448 508 KB  ](https://cdn3.ldstatic.com/original/4X/0/7/5/0754a494bf39c9e82b35816243492408e3860582.jpeg "image") |

### 错位矩形风格第一版

```markdown
生成一张 偶像大师闪耀色彩 的 樱木真乃 的人物海报。故障艺术风格，赛博朋克动漫美学，数字碎片化构图。画面由多个错位的矩形窗口和几何切片叠加而成，呈现出一种数据损坏和图像溢出的视觉感。核心风格包含：像素排序（Pixel Sorting）效果、RGB色彩偏移、横向拉伸的数字噪点以及彩虹色调的电流纹理。背景采用极简主义的米白色，与画面中心高饱和度的湛蓝天空、厚重的积雨云形成强烈视觉对比。整体氛围带有超现实的忧郁感和深邃的数字空间感，构图错落有致，充满现代平面设计感。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![image](https://cdn3.ldstatic.com/optimized/4X/3/d/4/3d44fcff68b904efccfb9296afa25e1dfc585ced_2_375x500.jpeg)  image1086×1448 679 KB  ](https://cdn3.ldstatic.com/original/4X/3/d/4/3d44fcff68b904efccfb9296afa25e1dfc585ced.jpeg "image") | [![image](https://cdn3.ldstatic.com/optimized/4X/4/4/6/4464b9c897f646935f7473e28f82c46f20b9227a_2_353x500.jpeg)  image1054×1492 520 KB  ](https://cdn3.ldstatic.com/original/4X/4/4/6/4464b9c897f646935f7473e28f82c46f20b9227a.jpeg "image") |

### 错位矩形风格第二版

```markdown
二次元平面艺术插画，角色为 偶像大师 的 如月千早。人物的衣服、动作、表情均可以替换。人物需要尽量使用全身像，且不使用常规的正面全身像而是做出展现人物动态的速写动作。画面采用“窗口重叠 (Window Overlay)”与“数字拼贴”的构图。角色的轮廓由多个错位的矩形框构成，某些方框区域被处理成透明视窗，展示出清朗的蓝天与积雨云纹理，仿佛角色体内蕴含着广阔的天空。画面中装饰有精美的故障艺术 (Glitch Art) 元素，如极简的黑色几何长条、细密的彩色电子扫描线以及错位的色彩偏移纹理。整体视觉呈现出一种现代平面设计的律动感，色彩以克莱因蓝和纯净白为主，背景简洁明快，氛围宁静且富有诗意。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![19f4bf070f608cdc32ecfd769b1c7bf1](https://cdn3.ldstatic.com/optimized/4X/1/f/0/1f03d8357316ed685f7dec0040f95d694da8a1e1_2_353x500.jpeg)  19f4bf070f608cdc32ecfd769b1c7bf11054×1492 393 KB  ](https://cdn3.ldstatic.com/original/4X/1/f/0/1f03d8357316ed685f7dec0040f95d694da8a1e1.jpeg "19f4bf070f608cdc32ecfd769b1c7bf1") | [![image](https://cdn3.ldstatic.com/optimized/4X/b/8/c/b8c3391d172b86ca5da2a8818a87bb9c5b34dbe8_2_375x500.jpeg)  image1086×1448 282 KB  ](https://cdn3.ldstatic.com/original/4X/b/8/c/b8c3391d172b86ca5da2a8818a87bb9c5b34dbe8.jpeg "image") |

### 混合媒介-照片+素描

```markdown
一件混合媒介艺术作品。前景色： 一个极简主义的白色线稿素描，描绘的是 偶像大师闪耀色彩 的 田中摩美美，近景胸像，线条细腻纤细，半透明的剪影感，全身仅眼睛部分带有 发光的淡紫色。人物的衣服、动作、表情均可替换为更适合整体风格的。背景： 一张写实的、大光圈虚化的摄影照片，场景为 黄昏时分的海岸电车道口与背后的海岸，电影感光影，天空呈现暮蓝色与金黄色的渐变。采用倾斜构图（荷兰角视角），水平线明显倾斜。风格： 空灵的氛围，怀旧的Lo-fi美学，锐利的白色线条与柔软模糊的实景摄影形成强烈对比，梦幻且忧郁的意境。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![image](https://cdn3.ldstatic.com/optimized/4X/b/a/2/ba21c4b93ed7bd1444afa261c2a28843ea1f553c_2_333x500.jpeg)  image853×1280 206 KB  ](https://cdn3.ldstatic.com/original/4X/b/a/2/ba21c4b93ed7bd1444afa261c2a28843ea1f553c.jpeg "image") | [![image](https://cdn3.ldstatic.com/optimized/4X/1/4/6/1461a7fcd74d29ac3ac5b4e41176e7c28f40ae31_2_500x500.jpeg)  image1254×1254 306 KB  ](https://cdn3.ldstatic.com/original/4X/1/4/6/1461a7fcd74d29ac3ac5b4e41176e7c28f40ae31.jpeg "image") |

### 黑蓝红三色

```markdown
极简主义平面插画风格，高对比度视觉冲击。画面以[背景颜色，如：鲜红色]为底色，采用[填入颜色，如：黑、白、红]三色限定。
【核心构图】：画面采用极强的对角线构图，以倾斜的地平线为视觉分界线，将空间切割为两个截然不同的色块区域：上方填充高饱和底色，下方呈现斑驳的浅色地表。
主体： 画面[方位，如：左下方]站立着[主体描述，例如：一个披着白色斗篷、银色长发的少女剪影]，呈现出纯净、发光的质感，轮廓跨越或靠近对角线。
环境： 背景中有一棵[环境核心，例如：巨大的炭黑色枯萎古树]，枝干呈放射状跨越对角线向四周延伸。树干带有[材质细节，如：水墨晕染与斑驳的裂纹]质感。
点缀与细节： [点缀物描述，例如：枝头停歇着几只纯白的飞鸟]。下方的地表呈现为[地面描述，例如：大面积斑驳的银白色荒原]，带有[纹理描述，如：粗糙的矿物颗粒感和干笔刷痕迹]。
艺术表现： 电影感广角比例，强烈的二次元平面感与写实纹理相结合。整体氛围呈现出一种[氛围关键词，如：孤独、神圣、超现实]的意境，线条锋利。
```

[![image](https://cdn3.ldstatic.com/optimized/4X/e/d/4/ed40044716f8a0f7421f6ce4feba47dc9a110d0d_2_517x345.jpeg)

image1536×1024 329 KB

](https://cdn3.ldstatic.com/original/4X/e/d/4/ed40044716f8a0f7421f6ce4feba47dc9a110d0d.jpeg "image")

### 半调双色雕刻风格

```markdown
一幅极简主义平面设计海报，采用“半调雕刻线稿”风格（Engraving Halftone Style）。画面由密集的[线条形状：如“同心圆”或“平行弧线”]构成，通过线条的粗细变化和疏密程度，巧妙地勾勒出[主体人物/对象：例如“一个侧脸的女性廓形”]的轮廓与面部阴影，形成强烈的立体感。视觉表现上采用极简双色调方案，背景色为[背景颜色：例如“深蓝色”]，线条颜色为[线条颜色：例如“明黄色”]。整体构图简洁有力，具有矢量艺术的质感，风格前卫且具有现代主义海报设计感。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![image](https://cdn3.ldstatic.com/optimized/4X/2/1/a/21a284c1232f43f9e333324e4371c4e17e7ed6b1_2_375x500.jpeg)  image1086×1448 696 KB  ](https://cdn3.ldstatic.com/original/4X/2/1/a/21a284c1232f43f9e333324e4371c4e17e7ed6b1.jpeg "image") | [![721f425f82bbbd3f8a66941c32404469](https://cdn3.ldstatic.com/optimized/4X/d/f/6/df6412044f972642a336985d78c9fb59a0b2039e_2_375x500.jpeg)  721f425f82bbbd3f8a66941c324044691086×1448 738 KB  ](https://cdn3.ldstatic.com/original/4X/d/f/6/df6412044f972642a336985d78c9fb59a0b2039e.jpeg "721f425f82bbbd3f8a66941c32404469") |

### 半调杂志风格

```markdown
现代复古平面海报设计，Risograph半调网点印刷风格。画面正中心是 [在此填写您的主体，例如：一只复古留声机 / 一把电吉他 / 一杯咖啡] 。主体采用深蓝与米白交织的半调网点纹理表现。背景为带有粗糙颗粒感的米色纸张。主体背后衬托着一个明黄色的几何实心拱门色块。主体周围环绕着极细的抽象交错轨道线条和几个微小的品红色四芒星符号。画面边缘（顶部和底部）带有深蓝色的复古粗体无衬线排版文字，部分文字带有明黄色高光色块底色。右上角包含一个条形码图形元素。整体构图极简，色彩对比强烈，具有波普艺术和复古杂志封面的视觉冲击力。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![image](https://cdn3.ldstatic.com/optimized/4X/6/b/1/6b1ae8e1715279310e83aeebfa81953b67d6f1d5_2_353x500.jpeg)  image1054×1492 855 KB  ](https://cdn3.ldstatic.com/original/4X/6/b/1/6b1ae8e1715279310e83aeebfa81953b67d6f1d5.jpeg "image") | [![image](https://cdn3.ldstatic.com/optimized/4X/e/c/e/ecec6427984525bae909669e6ad5eb08891419a5_2_374x500.jpeg)  image1085×1450 593 KB  ](https://cdn3.ldstatic.com/original/4X/e/c/e/ecec6427984525bae909669e6ad5eb08891419a5.jpeg "image") |

### 波普+水墨喷溅

```markdown
现代日系混合媒介插画风格，[在此处替换为您想要生成的主体内容]。
采用倒置动态构图，结合扁平化波普艺术逻辑。色彩以高饱和度明黄为主基调，运用克莱因蓝与大红进行强视觉对冲。画面融合赛璐璐平涂、波点网纹（Halftone）及水墨喷溅质感，具有纸张肌理与数码后期叠加的综合材质感。光影利落，空间呈现多层次平面拼贴关系。整体氛围洋溢着现代都市的轻盈感与瞬时爆发力，充满时尚平面设计的高信息密度与符号化视觉冲击。
```

[![image](https://cdn3.ldstatic.com/optimized/4X/e/6/e/e6e97387826560d52b356676922aeba2fc040a47_2_281x500.jpeg)

image941×1672 754 KB

](https://cdn3.ldstatic.com/original/4X/e/6/e/e6e97387826560d52b356676922aeba2fc040a47.jpeg "image")

### 看门狗-DEDSEC

```markdown
[在此处替换为您想要生成的主体内容]放置在画面正中央，作为绝对的视觉焦点。四周边缘有多只风格化、带有惊悚感的手臂呈放射状向中心抓取，前景的手部经过夸张的广角畸变处理被极度放大，产生强烈的透视压迫感与定格的侵入张力。整体画面呈现出硬核朋克、地下独立漫画与波普拼贴艺术相融合的美学风格，散发出躁动、反叛与赛博黑客般的地下氛围。
画面的色彩被严格限制在极高对比度的纯黑、纯白与高饱和度的亮橙色之中。光影被彻底扁平化处理，物体的体积与阴影完全依靠粗犷锐利的黑色墨线勾勒以及大面积、密集的半色调网点（Halftone patterns）来表现。背景由撕裂的纸张边缘、粗糙的数字噪点、斑驳的印刷纹理与黑橙相间的抽象几何色块堆叠而成，信息密度极高且无明显留白。强烈的丝网印刷质感与破坏性的层叠拼贴手法交织，营造出极具视觉冲击力的平面图形艺术效果。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![ddfb070f41ae27c3546c91798b55397e](https://cdn3.ldstatic.com/optimized/4X/2/8/5/2858770943a616c388c1815d5872ff4e3b3d2792_2_500x500.jpeg)  ddfb070f41ae27c3546c91798b55397e1254×1254 929 KB  ](https://cdn3.ldstatic.com/original/4X/2/8/5/2858770943a616c388c1815d5872ff4e3b3d2792.jpeg "ddfb070f41ae27c3546c91798b55397e") | [![fed088553ce71b75f7986244a56cd5fe](https://cdn3.ldstatic.com/optimized/4X/f/2/f/f2f27bf3a4e4b40598dd8a40242b603e71e44575_2_500x500.jpeg)  fed088553ce71b75f7986244a56cd5fe1254×1254 962 KB  ](https://cdn3.ldstatic.com/original/4X/f/2/f/f2f27bf3a4e4b40598dd8a40242b603e71e44575.jpeg "fed088553ce71b75f7986244a56cd5fe") |

### 克莱因秩序

```markdown
现代极简主义二次元插画，[在此处替换为您想要生成的动漫角色]，赛璐璐风格（Cel-shading）。画面采用极简的几何切割构图，角色置于大面积的负空间留白之中。色彩上采用极具冲击力的克莱因蓝（Klein Blue）与高亮纯白构成双色视觉核心。光影特质为硬边阴影（Hard edges shadow），模拟正午强烈的直射日光，角色受光面清透微曝，阴影区深邃且边缘锐利，呈现出极高的明暗对比度。空间逻辑采用强烈的仰拍透视，强调线条的延伸感。整体氛围具有一种夏日清冷、孤独且超现实的现代美感。线条利落，色彩平整，无杂色颗粒，通透感，大师级动画分镜感。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![814927c379ad874f96a64e0be562c981](https://cdn3.ldstatic.com/optimized/4X/9/7/1/97103a6a4f6c1dd15ec80c215c8009ff7beaf7d3_2_500x500.jpeg)  814927c379ad874f96a64e0be562c9811254×1254 173 KB  ](https://cdn3.ldstatic.com/original/4X/9/7/1/97103a6a4f6c1dd15ec80c215c8009ff7beaf7d3.jpeg "814927c379ad874f96a64e0be562c981") | [![image](https://cdn3.ldstatic.com/optimized/4X/5/1/9/519ef31a9ec1a9a8fda824d1ece88b1cfefc17da_2_500x500.jpeg)  image1254×1254 168 KB  ](https://cdn3.ldstatic.com/original/4X/5/1/9/519ef31a9ec1a9a8fda824d1ece88b1cfefc17da.jpeg "image") |

### 高对比度数字工业故障

```markdown
极简高对比图形艺术风格，[在此处替换为您想要生成的主体内容] 呈现出深邃的黑色剪影与鲜明电光蓝（Electric Blue）交织的重影质感。画面采用极端的仰视低角度构图（Low Angle Shot），展现强烈的动态对角线张力与线条穿插的复杂结构。背景为大面积的纯白高调留白，形成极高的视觉反差。色彩方案严格限定于：纯黑、克莱因蓝/电光蓝、以及高亮白。画面带有浓郁的胶片噪点、Riso印刷纹理、以及明显的色差边缘（Chromatic Aberration）与数字故障痕迹。光影呈现高阈值的二值化硬核特质，边缘锐化且伴有像素撕裂感。整体视觉语言融合了后现代工业美学与都市孤寂感，信息密度极高且富有冷峻的平面设计感，呈现出一种瞬时的、数字化的视觉定格。
```

| 测试用例1 | 测试用例2 |
| --- | --- |
| [![image](https://cdn3.ldstatic.com/optimized/4X/c/c/d/ccd4aa12be98e9072b92dd204266f1dfdc29f468_2_500x500.jpeg)  image1254×1254 778 KB  ](https://cdn3.ldstatic.com/original/4X/c/c/d/ccd4aa12be98e9072b92dd204266f1dfdc29f468.jpeg "image") | [![image](https://cdn3.ldstatic.com/optimized/4X/f/c/7/fc7c66b1d8276e7d2b1f213b4d12d0d7e6eeb18c_2_500x500.jpeg)  image1254×1254 791 KB  ](https://cdn3.ldstatic.com/original/4X/f/c/7/fc7c66b1d8276e7d2b1f213b4d12d0d7e6eeb18c.jpeg "image") |

## 怎样写出自己想要的没有的风格

其实无非就是两条路：去找到对应看风格的术语描述、从图片反推生图prompt。

现在学习对应的风格其实已经很简单了，直接让grok帮你搜一下历史到现代发展过程中所有有重大影响的设计风格，比如什么**瑞士风格、包豪斯、极简主义、极繁主义、超现实主义、至上主义、构成主义、半调风格、拼贴风格**……他总结好了，你带着这些关键词去google也好，还是去**Pinterest**搜关键词看图也罢。找到你心仪的风格，记住这个词，下次写提示词的时候就能带上了。

另外就是从图片反推prompt。比较适用于你本身自己就有看设计杂志或者在X还是P站刷图的人，给张图让gemini自己去用一段完整的自然语言概括风格就行。如果生出来不满意就回去gemini让他修改提示词就行了。

~~我自己用的一个反推提示词没怎么写，但是上面这些都是反推出来的。~~ 优化了一下新版的提示词：

```markdown
**请作为一名顶级的 AI 绘画提示词专家，为我分析这张图片的视觉风格。**

**任务目标：**
提取并反推这张图片的艺术风格，生成一份通用的 Prompt。这份 Prompt 必须剥离原图中的具体角色、文字或特定情节，仅保留其美学灵魂。

**分析维度（请务必涵盖以下 15 个方面）：**
1. **基础维度：** 画面风格、画面成分组成、构图方式、分镜类型、光影特质、色调与色彩科学、媒介与材质纹理、情绪与氛围、渲染/拍摄参数。
2. **进阶维度：** 时代感与文化语境、空间逻辑与透视关系、信息密度与留白、动态状态（瞬时感）、后期处理与数字痕迹、符号化特征。

**输出要求：**
1. 请直接输出一段完整的、高水准的**中文提示词**。
2. 在提示词的开头或核心位置，使用 **\`[在此处替换为您想要生成的主体内容]\`** 作为占位符。
3. 确保该 Prompt 具有高度通用性，用户只需更换占位符内容，即可在保持原图质感的同时生成全新的画面。
4. 无需输出分析过程，请直接给出最终的 Prompt 文本。
```

> 这里是旧版的提示词
> 
> ```markdown
> 反推生成这张图片的提示词，要求仅提取图片风格，生成一份通用的prompt，可以由用户自行决定生成主体内容，并且在prompt给出占位文字让用户自行替换。提取画面风格、组成元素、构图等等甚至更多详细内容。最终输出一段完整的中文prompt。
> ```

> 当然！我们为什么不弄个skill呢！不想用agent的话复制一下主体内容就好了，效果更好！

[SKILL.txt](https://linux.do/uploads/short-url/blBNJ7DvTIoXdDMOCHH4Xm1laPD.txt) (6.1 KB)

基本上以上就是全部的内容了。这几个Prompt其实如果被用多了也会烂大街，还是看自己有什么想法吧。GPT生图的能力本身就很强，但如果都用同样的Prompt看多了也会无聊。期待大家找到自己喜欢的风格并自己特化为Prompt下来。

## 题外话

What I am thinking……

![](https://cdn.ldstatic.com/user_avatar/linux.do/sallyn/48/1393867_2.png)

[通用焚决千篇一律，特殊风格万里挑一 | 一些非大流二次元向自用Prompt合集 | 一些自制焚决的思路](https://linux.do/t/topic/2044964/37) [搞七捻三](https://linux.do/c/gossip/11)> 说个题外话，技术上不一定行，只是个想法。可能需要oai或者google这种大厂才能做到了。 google前几天开源了他们 stitch 这个产品中用到的 DESIGN.MD 系统。这个系统是给 agent 一个写网站的约束，在里面会详细写设计网站需要尊重的风格和设定。 说不定未来可能哪家公司在生图上也能推出一个类似的约束系统呢，就叫什么 IMAGE.MD。输入图片，反推约束，特化成一个 IMA…

有能力的应该可以完善一下做个MVP出来2333

---

## Comments

> **coho** · [2026-04-24](https://linux.do/t/topic/2044964/2?u=lelele1)
> 
> ![](https://cdn.ldstatic.com/user_avatar/linux.do/sallyn/48/1393867_2.png) sallyn:
> 
> > 
> > ，给张图让 gemini 自己去用一段完整的自然语言概括风格就行
> 
> 对，让ai去给你解释，提供自然语言，比自己去摸索更容易一些。

> **coastisclear** · [2026-04-24](https://linux.do/t/topic/2044964/3?u=lelele1)
> 
> 感谢佬分享思路，看了几天出图确实渐渐麻木了。尤其是二次元的很多联动海报插画，很多图看下来感觉是炼了MJ导致画面大面积采用鳞片式上色的伪高级感（大面积的白点和头皮屑一样）。解决办法也比较简单，提供参考图在参考图基础上重新生图，GPT2的参考能力我目前使用下来感觉优于香蕉（提供人物照片做参考生成数字人角色）

> **linyuan1** · [2026-04-24](https://linux.do/t/topic/2044964/4?u=lelele1)
> 
> 哇哦，感谢佬分享的焚决，生成的图片真的好看有质感

> **HLiny** · [2026-04-24](https://linux.do/t/topic/2044964/5?u=lelele1)
> 
> ![](https://cdn.ldstatic.com/user_avatar/linux.do/sallyn/48/1393867_2.png) sallyn:
> 
> > 
> > 搜一下历史到现代发展过程中所有有重大影响的设计风格
> 
> 感谢佬友分享，这算不算是meta焚诀？看起来GPT什么风格都能拿捏啊

> **sallyn** · [2026-04-24](https://linux.do/t/topic/2044964/6?u=lelele1)
> 
> ![](https://cdn.ldstatic.com/user_avatar/linux.do/coastisclear/48/1718374_2.png) 初号机抑制器:
> 
> > 
> > 看了几天出图确实渐渐麻木了。尤其是二次元的很多联动海报插画
> 
> 哈哈哈 刚开始白天还挺好玩儿的 到了晚上大家做的无非上就是内容和梗的区别了 有些审美疲劳
> 
> ![](https://cdn.ldstatic.com/user_avatar/linux.do/coastisclear/48/1718374_2.png) 初号机抑制器:
> 
> > 
> > GPT2的参考能力我目前使用下来感觉优于香蕉（提供人物照片做参考生成数字人角色）
> 
> 是这样滴 风格迁移上也比![:banana:](https://cdn.ldstatic.com/images/emoji/twemoji/banana.png?v=15 ":banana:")强上很多
> 
> ---
> 
> 我还有几个电影海报的迁移 不得不说有些经典电影或者专辑的设计也挺有意思 这些也挺适合抽取出来的
> 
> | 原作 | GPT |
> | --- | --- |
> | [![image](https://cdn3.ldstatic.com/original/4X/0/a/5/0a5d118b44601b32f8617d37f1a23f877c37ffe7.jpeg)  image259×383 19.6 KB  ](https://cdn3.ldstatic.com/original/4X/0/a/5/0a5d118b44601b32f8617d37f1a23f877c37ffe7.jpeg "image") | [![image](https://cdn3.ldstatic.com/optimized/4X/d/a/1/da19d220227332fdf5a46da5cbd7b89613e17d30_2_373x500.jpeg)  image484×648 70.8 KB  ](https://cdn3.ldstatic.com/original/4X/d/a/1/da19d220227332fdf5a46da5cbd7b89613e17d30.jpeg "image") |
> 
> > 出自电影《猫鼠游戏》