---
title: "全套APK逆向/前端JS逆向套件和工程方法论skill"
source: "https://linux.do/t/topic/2142539"
author:
  - "[[hisence]]"
published:
created: 2026-05-15
description: "近期发的一些逆向帖子，有很多佬友都在问逆向用的工具之类的，这里和大家分享一下自用的逆向开发环境。 deepseek v4 逆向出奇的好用 开发调优, Lv1 利用 v4 f"
tags:
  - "clippings"
---
近期发的一些逆向帖子，有很多佬友都在问逆向用的工具之类的，这里和大家分享一下自用的逆向开发环境。

![](https://cdn.ldstatic.com/user_avatar/linux.do/hisence/48/1778165_2.png)

[deepseek v4 逆向出奇的好用](https://linux.do/t/topic/2082605) [开发调优, Lv1](https://linux.do/c/develop/develop-lv1/20)

> 利用 v4 flash 逆向一个网站的 加密下载接口，一顿操作猛如虎，工具调用丝滑，几十轮的抓包没有一次报错，仅仅不到五分钟完全破解登录 POW 密钥和隐藏下载接口。 最牛逼的是，不用任何提示词引导，直接就说逆向破解，有啥说啥，ds 根本没有道德限制，沟通成本 0![laughing](https://cdn.ldstatic.com/images/emoji/twemoji/laughing.png?v=15 "laughing")![laughing](https://cdn.ldstatic.com/images/emoji/twemoji/laughing.png?v=15 "laughing") [\[mmexport1777458054496.jpg\]](https://cdn3.ldstatic.com/original/4X/8/4/e/84e86174869d3e5fea922e85f66e4ffdd721e45f.jpeg "mmexport1777458054496.jpg") 成本 2 毛 5。…

---

### 终端工具: opencode

### 模型: ds v4

### 提示词：ds 不带甲，直接说需求，opencode 提示词没有安全引导，cc 可能默认提示词里带一些甲，需要稍微绕一下。

---

### 通用 GUI：

[通用抓包 anything-analyzer](https://github.com/Mouseww/anything-analyzer)

---

### MCP 类：

[前端逆向js-reverse-mcp](https://github.com/zhizhuodemao/js-reverse-mcp)  
[二进制解包/反混淆逆向类ida-pro-mcp](https://github.com/mrexodia/ida-pro-mcp)  
[浏览器自动化操作 playwright-mcp](https://github.com/microsoft/playwright-mcp)

---

### cli 工具：

[APK静态编译/smali修改-- jadx](https://github.com/skylot/jadx)  
[APK解包/签名/打包工具-- Apktool](https://github.com/iBotPeaches/Apktool)  
[动态编译/分析/hook工具-- frida](https://github.com/frida/frida)  
安卓 SDK 开发套件 ADB/apksigner（自行下载）  
[解包cli工具，更加精细/批量-- radare2](https://github.com/radareorg/radare2)

---

### 自用/整理出的配套 skill

[skills.zip](https://linux.do/uploads/short-url/oT5VLgII3Qvhq4Omxy87sVje3ZY.zip) (177.2 KB)

- apk-reverse : **APK 分析全流程方法指导**
- mcp-js-reverse-playbook ：**前端 JS 逆向方法论指导**
- ida-reverse : **IDAPRO 工具使用方法论**
- radare2 : **radare2 cli 工具使用方法论**
- reverse-engineering : 工**程专业化逆向指导全套工作流和部分CTF题库案例**

注意：skill 是自己使用创建的，部分脚本可能硬编码了我的电脑路径，建议先让 AI 审核修改一下。