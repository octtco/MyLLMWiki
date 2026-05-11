---
title: "给大家公开一个无限撸4.7，并且可以中转的路子"
source: "https://linux.do/t/topic/2028876"
author:
  - "[[DUODUSHU]]"
published:
created: 2026-04-22
description: "第一次写，然后在站内看到有些大佬分享了关于windsurf的试用资格，也看到了一些大佬分享了关于windsurf的pro号额度。今天分享一下市面号商windsurf试用号起号的方法。只分享思路，注册机暂时不开源。 1，看到各位佬说有注册没有支付宝方式，其实可以切换新加坡IP去登录"
tags:
  - "clippings"
---
> **第一次写，然后在站内看到有些大佬分享了关于windsurf的试用资格，也看到了一些大佬分享了关于windsurf的pro号额度。今天分享一下市面号商windsurf试用号起号的方法。只分享思路，注册机暂时不开源。**
> 
> 1，看到各位佬说有注册没有支付宝方式，其实可以切换新加坡IP去登录官网然后记得抓包网站Export HAR文件，然后交给AI去解析，后面获得自己的plan=\*的登录方式，反复使用相同链接进入官网，然后每一个都会包含试用（这里要提醒的是wf的官网会记录你的cookie以及浏览器的内核，多次注册会被标记，所以我建议使用指纹浏览器，我个人使用的比特浏览器，自己去官网下载就好了，懂指纹浏览器的就不需要过多介绍了，自己研究一下）然后关于解析的问题，可能有些佬连解析都感觉费劲，我就放一个我个人解析的带试用的链接（不需要看当前IP）： [https://windsurf.com/account/register?redirect\_uri=%2Fbilling%2Findividual%3Fplan%3D9](https://windsurf.com/account/register?redirect_uri=%2Fbilling%2Findividual%3Fplan%3D9)
> 
> 2，关于注册邮箱的问题，在wf种会有一些邮箱不能使用4.7 4.6 模型，这边推荐gmail. asia .以及online，这些是当前闲鱼号商比较普遍的邮箱，如果你不确定到底哪些邮箱可以使用，可以去闲鱼买一个能用4.7的试用号看一下邮箱结尾，然后可以启用相关的域名邮箱来进行注册。
> 
> 3，关于支付方式，支付宝扫码记得及时取消订阅，我走的是实体visa卡进行的相关订阅，我自己测试的支付宝注册了4-5个，没有被判定风险，但是我后面还是使用了相关的实体卡（这里也希望各位佬能分享一下可用的卡头，虚拟卡我试过也能通过，但是我个人使用卡有限）
> 
> 4.支付成功之后就到了我们接下来反代中转了，这边走的一个佬的开源反代项目：[https://github.com/guanxiaol/WindsurfPoolAPI](https://github.com/guanxiaol/WindsurfPoolAPI) ，然后可以部署在服务器上面，进行响应的模型请求映射，这个跟sub2api一个性质都是号池，然后配置好响应请求。自带缓存，做中转的佬记得配置好自己中转的缓存。
> 
> [![image](https://cdn3.linux.do/optimized/4X/6/9/0/690db9b44e5c12c1c1b9bbfb62082c06ccf204b7_2_690x315.png)
> 
> image1920×879 51.5 KB
> 
> ](https://cdn3.linux.do/original/4X/6/9/0/690db9b44e5c12c1c1b9bbfb62082c06ccf204b7.png "image")
> 
> [![image](https://cdn3.linux.do/optimized/4X/d/2/1/d2168a0aee3e7a6d389193abbd641742c67aecec_2_690x351.png)
> 
> image1590×810 57 KB
> 
> ](https://cdn3.linux.do/original/4X/d/2/1/d2168a0aee3e7a6d389193abbd641742c67aecec.png "image")
> 
> [![image](https://cdn3.linux.do/optimized/4X/2/3/0/230cf7c74fb0ead74ae888a18c701b06a0f635b9_2_624x500.png)
> 
> image981×785 62.3 KB
> 
> ](https://cdn3.linux.do/original/4X/2/3/0/230cf7c74fb0ead74ae888a18c701b06a0f635b9.png "image")
> 
> 基本上思路就是这样，这条路可以做两种，1做4.7中转商 2做试用号商，写的有点笼统，只是简单的分享一下思路，具体操作可以交给AI。

---

## Comments

> **hyruur** · [2026-04-22](https://linux.do/t/topic/2028876/2?u=lelele1)
> 
> 有没有人用0刀卡去绑定， windsurf大善人能持续多久

> **DUODUSHU** · [2026-04-22](https://linux.do/t/topic/2028876/3?u=lelele1)
> 
> 我试的bybit的U卡可以，关于封号的问题，我还真没遇到

> **xingxing01** · [2026-04-22](https://linux.do/t/topic/2028876/4?u=lelele1)
> 
> 主要是买了，中转了之后，蹬起来了，蹬的正兴奋时候，号又被干了，能蹬多久? 应该没法保证吧

> **yetong1234** · [2026-04-22](https://linux.do/t/topic/2028876/5?u=lelele1)
> 
> 活不了多久的，加快死亡，希望不要影响正常用户