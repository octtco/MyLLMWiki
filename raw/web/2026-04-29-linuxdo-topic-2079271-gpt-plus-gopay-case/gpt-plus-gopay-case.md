---
title: "GPT Plus 道爷我成了（GoPay版本）"
source: "https://linux.do/t/topic/2079271"
author:
  - "[[zzzxdm]]"
published:
created: 2026-04-29
description: "前人栽树，感谢这些佬 https://linux.do/t/topic/2076911 https://linux.do/t/topic/2077544 说说我的操作过程 1、iPhone下载whatsapp和gopay 2、注册whatsapp，+86手机号收不到验证码，用的t"
tags:
  - "clippings"
---
前人栽树，感谢这些佬  
[https://linux.do/t/topic/2076911](https://linux.do/t/topic/2076911)  
[https://linux.do/t/topic/2077544](https://linux.do/t/topic/2077544)  
**说说我的操作过程**  
1、iPhone下载whatsapp和gopay  
2、注册whatsapp，+86手机号收不到验证码，用的talkatone美国号（竟然能接码）  
3、注册gopay，用talkatone美国号，whatsapp接码。设置pin，不会问gpt，我也看不懂印度尼西亚语  
4、开薅gpt plus，这个老生常谈的问题了  
送你们一个脚本，一键直达GoPay开通页面

```javascript
javascript:(async function(){try{const s=await(await fetch("/api/auth/session")).json();if(!s.accessToken){alert("请先登录 ChatGPT！");return}const p={"entry_point":"all_plans_pricing_modal","plan_name":"chatgptplusplan","billing_details":{"country":"ID","currency":"IDR"},"promo_campaign":{"promo_campaign_id":"plus-1-month-free","is_coupon_from_query_param":false},"checkout_ui_mode":"custom"},r=await fetch("https://chatgpt.com/backend-api/payments/checkout",{method:"POST",headers:{Authorization:"Bearer "+s.accessToken,"Content-Type":"application/json"},body:JSON.stringify(p)}),d=await r.json();d.checkout_session_id?window.location.href="https://chatgpt.com/checkout/openai_llc/"+d.checkout_session_id:alert("提取失败："+(d.detail||JSON.stringify(d)))}catch(e){alert("发生错误："+e)}})();
```

**全程不要一分钱，接码都省了…**  
**不需要印尼节点**

---

## Comments

> **typer** · [2026-04-29](https://linux.do/t/topic/2079271/2?u=lelele1)
> 
> 可以的佬友，很强啊哈哈哈哈，学习一下。 ![:grinning_face:](https://cdn.ldstatic.com/images/emoji/twemoji/grinning_face.png?v=15 ":grinning_face:")

> **sky** · [2026-04-29](https://linux.do/t/topic/2079271/3?u=lelele1)
> 
> 佬不用印尼节点吗？我现在还在抓印尼节点。

> **zzzxdm** · [2026-04-29](https://linux.do/t/topic/2079271/4?u=lelele1)
> 
> 不用什么印尼节点，没要求吧好像，我是日本的IP