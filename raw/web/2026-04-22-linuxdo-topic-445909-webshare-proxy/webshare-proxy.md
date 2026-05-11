---
title: "webshare.io家宽包年8美元与clash链式代理部署教程，可以一定程度解决ChatGPT降智与注册较高风控账号"
source: "https://linux.do/t/topic/445909"
author:
  - "[[msm8976]]"
published:
created: 2026-04-22
description: "年前由于ChatGPT降智参考了论坛的帖子买了webshare的低价家宽，购买和部署的过程中发现了一些可以改进的方式，来分享一下自己的使用经验 省流与免责声明 webshare家宽相当于每年不到10刀买一台较纯净ip的socks5落地代理，需要外卡支付并搭配已有出国节点使用"
tags:
  - "clippings"
---
年前由于ChatGPT降智参考了[论坛的帖子](https://linux.do/t/topic/271623)买了webshare的低价家宽，购买和部署的过程中发现了一些可以改进的方式，来分享一下自己的使用经验

# 省流与免责声明

1. webshare家宽相当于每年不到10刀买一台较纯净ip的socks5落地代理，需要外卡支付并搭配已有出国节点使用
2. 本人使用的是Windows系统下[clash-verge](https://github.com/clash-verge-rev/clash-verge-rev)软件，不同系统与软件可能存在一定差异
3. 该教程仅为本人经验分享，不保证完全正确，若存在问题欢迎评论指正
4. 家宽代理只能一定程度上解决降智，具体风控策略与ip、账号、使用频率等均相关，建议先买一个月测试再买包年

# 具体教程

## 注册webshare家宽

[Webshare | Fast & Affordable Proxies](https://www.webshare.io/?referral_code=52hjyi0yce0r) [AFF](https://linux.do/tag/AFF)

若此前注册过账号直接登录（老号价格可能更便宜），推荐使用谷歌账号注册，注册后会赠送10个代理ip不用管直接进主界面即可

## 订阅套餐

点击左侧订阅-浏览方案，选择静态住宅-私有，代理数量点开选自定义1个，带宽选250GB每月

[![套餐选择1](https://cdn3.linux.do/optimized/4X/d/c/4/dc4aafc12da3c732541d0643860c668a3d7a50cc_2_690x320.png)

套餐选择11897×880 121 KB

](https://cdn3.linux.do/original/4X/d/c/4/dc4aafc12da3c732541d0643860c668a3d7a50cc.png "套餐选择1")

此处带宽为走代理的流量，后续会通过Clash分流来限定仅白名单走家宽代理，250G肯定够用了

不建议全局走这个代理，大部分网站不会风控ip，且美国的延迟会更高，手动将需要家宽的网站加到白名单即可

国家推荐美国，若有特殊需求可自行选择，代理刷新前两个选不刷新，第三个自定义选20个刷新次数，额外特性不需要选

[![套餐选择2](https://cdn3.linux.do/optimized/4X/0/9/0/090e321ac9368287ac8afa667963f86294db6da9_2_690x350.png)

套餐选择21433×728 58.4 KB

](https://cdn3.linux.do/original/4X/0/9/0/090e321ac9368287ac8afa667963f86294db6da9.png "套餐选择2")

备注：若仅购买单月可选择22个，包年选择20个，这个数字是不加钱能选的最大数量，搭配后面选择ASN更换用不完，没必要加钱选50个

选好后右侧会显示价格，如果按照上述配置单月应为1美元，年付虽然显示-30%，但不同账号会有不同的折扣，我去年年底用谷歌注册的号是-33.3%包年就是8刀，新注册的号貌似都是-20%就是9.6刀

[![不同号价格](https://cdn3.linux.do/optimized/4X/2/3/8/2381c66d4a54c3aab641e3285016f1ece148793e_2_690x447.png)

不同号价格1044×677 44.8 KB

](https://cdn3.linux.do/original/4X/2/3/8/2381c66d4a54c3aab641e3285016f1ece148793e.png "不同号价格")

第一次使用建议买一个月即可，后续即使想要包年这1美元也不会浪费，直接买包年万一想退不一定好退

通过测试猜测的扣费规则是：每次创建订单会将完整的价格扣费并充值到余额，按天从余额扣款，后续更改套餐可以使用已有余额抵扣，所以如果用着感觉不错切换到包年这1刀是可以抵扣的

我付款用的是中行的莫奈万事达借记卡，对卡应该没有要求，只要是VISA、万事达、AMEX的就行

如果你有使用多个代理的需求（例如不同账号挂不同代理），建议注册多个账号每个账号买一个。同一个账号下的流量和刷新次数是共享的，例如你买了5个ip，平均每个ip每月就只能用50G流量和更换4次

## 测试代理

购买成功后，左侧代理列表里就可以看到代理信息，包含ip 端口 用户名 密码，如果对代理质量没有要求直接用就行，但还是建议通过以下方式测试并挑选代理，反正20次更换不用白不用

[![代理列表](https://cdn3.linux.do/optimized/4X/b/3/4/b3424d78065055354351d8a15e9999ce19ebe9ca_2_690x165.jpeg)

代理列表2430×582 112 KB

](https://cdn3.linux.do/original/4X/b/3/4/b3424d78065055354351d8a15e9999ce19ebe9ca.jpeg "代理列表")

### ip质量测试

一般而言我就看一下[ping0.cc](https://ping0.cc/)，只要没有显示IDC或者风控值特别高就可以，没必要追求所谓的双isp，毕竟ChatGPT用的也不是这个网站的风控，只要ChatGPT不降智就行

如果需要注册较高风控账号，或者用于直播电商等可以按照参考下面的帖子进一步测试，当然如果需求很高得加钱，这个每月1刀的大概率不行

![](https://linux.do/user_avatar/linux.do/7li7li/48/319449_2.png)

[教你如何辨别家宽](https://linux.do/t/topic/309732) [开发调优](https://linux.do/c/develop/4)

> 前言 自从ChatGPT降智和Claude风控问题开始，越来越多的人有了家宽需求。很多小伙伴喜欢用[ping0.cc](https://ping0.cc/)显示的IP类型 来做看家宽和ip纯净度。但ping0的家宽显示仅供参考（实际不值得参考），很多家宽显示机房，机房显示家宽就离谱，不如其他数据库准确。! ! [\[image\]](https://cdn3.linux.do/original/4X/1/3/7/137cda22f73ba3c9b64cc5008519ab0d07f655b0.png "image") 如何判断家宽（以ping0.cc为例） 家宽要素： ①ASN所有者 类型为ISP ②企业 类型为ISP …

### ChatGPT降智测试

降智有很多种测试方式，我一般用pow和4o/o3-mini两个问题来测试

#### pow测试

pow可以近似地理解为OpenAI对你ip的风控值，可以通过油猴脚本 [更好看的PoW检测（解除降智）脚本](https://linux.do/t/topic/290979) 或者浏览器调试的chat-requirements看

pow最理想的情况是在不模拟UA的情况下5位长度甚至7a120，但我只在一月的时候遇见过，最近不知道是不是风控策略更改不管怎么换ip不模拟UA都很难稳定5位。pow也只是提供参考，和是否降智不绝对相关

#### 问题测试

第一个问题，用普通的4o（非推理）：

> summarize your tools in markdown table with availability

如果结果只有1行bio就是降智，这时切换到4o-mini如果不止1行会比降智的4o更聪明

第二个问题，用o3-mini（推理），问题可以随便，只要不是太过于简单的就行，比如可以用我在 [一个推理模型很难回答出的简单问题，5.5米长的竹竿能否通过高4米宽3米的门](https://linux.do/t/topic/425230) 提到的：

> 5.5米长的竹竿，能否通过高4米宽3米的门，要求你认真思考，给出原理和答案。

观察回复UI，如果推理过程中类似于下图的新界面，每一步标题有光晕动画，内容较长（至少2行），且下一步推理时会覆盖此前的内容，最终推理完成展开推理过程时没有标题只有内容，即为未降智

[![未降智示例](https://cdn3.linux.do/optimized/4X/b/2/1/b213873b51c1385c5a491c8fb6f00afdf6579bbe_2_690x111.png)

未降智示例2032×327 52.9 KB

](https://cdn3.linux.do/original/4X/b/2/1/b213873b51c1385c5a491c8fb6f00afdf6579bbe.png "未降智示例")

如果是老界面，每一步是一个静态的加粗标题，内容较短，且推理过程中就完整的展示每一步的标题和内容，即为降智

这是以前其他问题的老图，之后遇到了降智再补新的  

[![降智示例](https://cdn3.linux.do/original/4X/8/b/c/8bc253ed48a71761e02eeed1641bb8f4d19007dd.png)

降智示例1125×410 20.2 KB

](https://cdn3.linux.do/original/4X/8/b/c/8bc253ed48a71761e02eeed1641bb8f4d19007dd.png "降智示例")

个人感觉按照降智概率而言o3-mini>4o>4o-mini，即某个账号可能o3-mini降了但4o没降，但没遇到过4o降了但o3-mini没降

## 更换代理

如果代理的风控值不满意，或者发现ChatGPT再次降智，可以更换代理  
首次默认分配的代理一般质量都不太行，除非风控值低且为双isp否则建议更换

在代理列表中勾选想要更换的代理ip（我买了2个，你们的界面应该是一个），点上方Replace进入更换界面

[![更换代理](https://cdn3.linux.do/optimized/4X/4/d/f/4df394472c8ac36146e4dc2ecdc8280dd537c192_2_690x137.jpeg)

更换代理2403×479 94.2 KB

](https://cdn3.linux.do/original/4X/4/d/f/4df394472c8ac36146e4dc2ecdc8280dd537c192.jpeg "更换代理")

第一步默认会选中你刚刚勾选的代理，下一步选择第二个从具体ASN中添加代理，推荐选择ATT（ASN7018）的

我基本上把所有的都测试了一遍，ATT的质量相对最好，也可以自己试一试其他的，注意这里是所有国家的，如果选了其他国家的ASN会变国家，ATT里都是美国的

[![选择ATT](https://cdn3.linux.do/optimized/4X/4/9/d/49d7156eb6e58bf0133f29f01ec84fd6aedb1ada_2_690x273.png)

选择ATT1989×789 41.4 KB

](https://cdn3.linux.do/original/4X/4/9/d/49d7156eb6e58bf0133f29f01ec84fd6aedb1ada.png "选择ATT")

然后下一步提交，更换后此前的代理会立刻无法使用，代理列表中会显示最新的代理，这时候就重新按照第三步测试，可以多次更换直到选到满意的ip

此外，除了选择ASN外，更换时还可以选择指定的ip号段，但ip号段只能选自己曾经随机到过的。购买时选择的20次更换次数会每月重置，因此在每月套餐即将结束时可以多刷新几次把刷新次数用完，并记录较好的ip号段指定更换

同时，欢迎各位佬在评论区发一下自已挑选后满意的ip号段（前两部分即可，例如我截图中的208.66.x.x），以及该ip测试的风控值

## 配置Clash分流与链式代理

链式代理指的是将请求通过多个ip依次中转，我们要让ChatGPT认为自己是家宽就得把家宽放到最后一个，V2等软件可能把这个功能叫做落地代理

首先在全局拓展脚本里粘贴下面的内容，并把ip端口用户名密码换成自己的，作用是把自己的家宽代理添加到节点列表中，当然也可以手动编辑订阅添加节点

```lua
function main(config, profileName) {
  const nodeList= 
  [
    {
      "name": "webshare",
      "server": "你的ip",
      "port": 你的端口,
      "type": "socks5",
      "username": "你的用户名",
      "password": "你的密码",
      "tls": false,
      "skip-cert-verify": true,
      // "udp": true
    },
  ]
  nodeList.forEach(node => {
    config.proxies.push(node);
  });
  return config;
}
```

然后在全局拓展配置中添加一个代理组，type为relay，proxies首先填自己的出国节点，然后再填webshare（上方我提供的拓展脚本里把节点命名为了webshare）

```yaml
- name: 链式代理
    type: relay
    proxies:
      - 低延迟
      - webshare
```

最后在全局拓展配置的分流规则中把需要家宽代理的分流到链式代理上

```markdown
rules:
  - RULE-SET,ai,链式代理
  - RULE-SET,AI,链式代理
  - RULE-SET,OpenAI,链式代理
  - RULE-SET,Gemini,链式代理
  - RULE-SET,Claude,链式代理
  - DOMAIN-SUFFIX,oaistatic.com,链式代理
  - DOMAIN-SUFFIX,cdn.oaistatic.com,链式代理
  - DOMAIN-SUFFIX,gstatic.com,链式代理
```

下面是我自己正在使用的完整全局扩展配置，算是整合了此前一些人的配置，没有过多特殊需求可以直接复制使用  
我的配置里没有给不同类别添加不同分流，只保留了普通代理和链式代理，如果有分流需求也可以在自己的基础上参考添加

```
# Profile Enhancement Merge Template for Clash Verge
proxy-groups:
  - name: 低延迟
    include-all: true
    type: select
    proxies:
      - 自动选择

  - name: 高带宽
    include-all: true
    type: select
    proxies:
      - 自动选择

  - name: 链式代理
    type: relay
    proxies:
      - 低延迟
      - webshare

  - name: 自动选择
    type: url-test
    include-all: true
    url: http://www.gstatic.com/generate_204
    interval: 1800

rule-providers:
  ai:
    type: http
    behavior: classical
    format: yaml
    path: ./rules/ai.yaml
    url: "https://fastly.jsdelivr.net/gh/MadisonWirtanen/WARP-Clash-with-ZJU-Rules@main/ai.yaml"
    interval: 86400

  AI:
    type: http
    behavior: classical
    url: https://github.com/Repcz/Tool/raw/X/Clash/Rules/AI.list
    path: ./rule-providers/AI.list
    interval: 86400
  
  OpenAI: 
    type: http
    behavior: classical
    format: yaml
    path: ./rules/OpenAI.yaml
    url: "https://cdn.jsdelivr.net/gh/zuluion/Clash-Template-Config@master/Filter/OpenAI.yaml"
    interval: 86400
    
  Gemini: 
    type: http
    behavior: classical
    format: yaml
    path: ./rules/Gemini.yaml
    url: "https://cdn.jsdelivr.net/gh/zuluion/Clash-Template-Config@master/Filter/Gemini.yaml"
    interval: 86400

  Claude: 
    type: http
    behavior: classical
    format: yaml
    path: ./rules/Claude.yaml
    url: "https://cdn.jsdelivr.net/gh/zuluion/Clash-Template-Config@master/Filter/Claude.yaml"
    interval: 86400

  AD:
    type: http
    behavior: classical
    url: https://adrules.top/adrules_domainset.txt
    path: ./rule-providers/AD.list
    interval: 86400

  AdBlock:
    type: http
    behavior: classical
    format: yaml
    path: ./rules/AdBlock.yaml
    url: "https://cdn.jsdelivr.net/gh/zuluion/Clash-Template-Config@master/Filter/AdBlock.yaml"
    interval: 86400
    
  BanAD:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanAD.list"
    path: ./ruleset/BanAD.yaml
    interval: 86400

  BanProgramAD:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanProgramAD.list"
    path: ./ruleset/BanProgramAD.yaml
    interval: 86400

  BanEasyList:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanEasyList.list"
    path: ./ruleset/BanEasyList.yaml
    interval: 86400

  reject:
    type: http
    behavior: domain
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/reject.txt"
    path: ./ruleset/reject.yaml
    interval: 86400

  collection: 
    type: http
    behavior: classical
    format: yaml
    path: ./rules/collection.yaml
    url: "https://gist.githubusercontent.com/cnfree8964/0864fd1d2e88936a095fb40d74ce4993/raw/collection.yaml"
    interval: 86400

  gfw:
    type: http
    behavior: domain
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/gfw.txt"
    path: ./ruleset/gfw.yaml
    interval: 86400

  proxy:
    type: http
    behavior: domain
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/proxy.txt"
    path: ./ruleset/proxy.yaml
    interval: 86400

  tld-not-cn:
    type: http
    behavior: domain
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/tld-not-cn.txt"
    path: ./ruleset/tld-not-cn.yaml
    interval: 86400

  ProxyGFWlist:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ProxyGFWlist.list"
    path: ./ruleset/BanEasyList.yaml
    interval: 86400

  ProxyClient: 
    type: http
    behavior: classical
    format: yaml
    path: ./rules/ProxyClient.yaml
    url: "https://cdn.jsdelivr.net/gh/zuluion/Clash-Template-Config@master/Filter/ProxyClient.yaml"
    interval: 86400

  ChinaDomain:
    type: http
    behavior: classical
    format: yaml
    path: ./rules/ChinaDomain.yaml
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaDomain.list"
    interval: 86400

  ChinaCompanyIp:
    type: http
    behavior: classical
    format: yaml
    path: ./rules/ChinaCompanyIp.yaml
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaCompanyIp.list"
    interval: 86400

  China: 
    type: http
    behavior: classical
    format: yaml
    path: ./rules/China.yaml
    url: "https://cdn.jsdelivr.net/gh/zuluion/Clash-Template-Config@master/Filter/China.yaml"
    interval: 86400

  cncidr:
    type: http
    behavior: ipcidr
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/cncidr.txt"
    path: ./ruleset/cncidr.yaml
    interval: 86400

  lancidr:
    type: http
    behavior: ipcidr
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/lancidr.txt"
    path: ./ruleset/lancidr.yaml
    interval: 86400

profile:
  store-selected: true

dns:
  enable: true
  ipv6: false
  listen: 0.0.0.0:53
  enhanced-mode: fake-ip
  fake-ip-range: 198.18.0.1/16
  nameserver:
  - https://doh.pub/dns-query
  - https://dns.alidns.com/dns-query
  prefer-h3: true
  nameserver-policy: # 国内的DNS服务器没必要使用doh/dot加密，不加密速度更快
    geosite:cn:
    # - system
    - 223.5.5.5
    - 114.114.114.114
    - 180.184.1.1
    - 119.29.29.29
    - 180.76.76.76
  proxy-server-nameserver: # 解析代理节点的DNS服务器
  - https://doh.pub/dns-query
  - https://dns.alidns.com/dns-query
  fallback: []
  fake-ip-filter: # fake-ip的副作用，导致Windows上会显示无网络，屏蔽微软的一些域名即可解决
  - '*.lan'
  - 'localhost.ptlogin2.qq.com'
  - 'localhost.sec.qq.com'
  - dns.msftncsi.com
  - www.msftncsi.com
  - www.msftconnecttest.com
unified-delay: true
tcp-concurrent: true

tun:
  enable: true
  stack: mixed
  auto-route: true
  auto-redirect: true
  auto-detect-interface: true
  dns-hijack:
    - any:53
    - tcp://any:53
  device: utun0
  mtu: 1500
  strict-route: true
  gso: true
  gso-max-size: 65536
  udp-timeout: 300
  iproute2-table-index: 2022
  iproute2-rule-index: 9000
  endpoint-independent-nat: false
  route-address-set:
    - ruleset-1
  route-exclude-address-set:
    - ruleset-2
  route-address:
    - 0.0.0.0/1
    - 128.0.0.0/1
    - "::/1"
    - "8000::/1"
  route-exclude-address:
    - 192.168.0.0/16
    - fc00::/7
  include-interface:
    - eth0
  exclude-interface:
    - eth1
  include-uid:
    - 0
  include-uid-range:
    - 1000:9999
  exclude-uid:
    - 1000
  exclude-uid-range:
    - 1000:9999
  include-android-user:
    - 0
    - 10
  include-package:
    - com.android.chrome
  exclude-package:
    - com.android.captiveportallogin

rules:
  - RULE-SET,ai,链式代理
  - RULE-SET,AI,链式代理
  - RULE-SET,OpenAI,链式代理
  - RULE-SET,Gemini,链式代理
  - RULE-SET,Claude,链式代理
  - DOMAIN-SUFFIX,oaistatic.com,链式代理
  - DOMAIN-SUFFIX,cdn.oaistatic.com,链式代理
  - DOMAIN-SUFFIX,gstatic.com,链式代理

  - DOMAIN-SUFFIX,googleapis.cn,低延迟
  - DOMAIN-SUFFIX,oncatapult.com,DIRECT
  - DOMAIN-SUFFIX,epicgames.com,DIRECT
  - DOMAIN-SUFFIX,linux.do,DIRECT

  - GEOSITE,category-ads-all,REJECT

  - RULE-SET,AD,REJECT
  - RULE-SET,AdBlock,REJECT
  - RULE-SET,reject,REJECT
  - RULE-SET,BanAD,REJECT
  - RULE-SET,BanProgramAD,REJECT
  - RULE-SET,BanEasyList,REJECT

  - GEOSITE,private,DIRECT
  - GEOIP,private,DIRECT,no-resolve

  - GEOSITE,category-scholar-!cn,低延迟
  - GEOSITE,microsoft@cn,DIRECT
  - GEOSITE,steam@cn,DIRECT
  - GEOSITE,category-games@cn,DIRECT
  - GEOSITE,cn,DIRECT
  - GEOIP,CN,DIRECT,no-resolve
  
  # - RULE-SET,gfw,低延迟
  # - RULE-SET,proxy,低延迟
  # - RULE-SET,tld-not-cn,低延迟
  # - RULE-SET,ProxyGFWlist,低延迟
  # - RULE-SET,ProxyClient,低延迟
  - RULE-SET,ChinaDomain,DIRECT,no-resolve
  - RULE-SET,ChinaCompanyIp,DIRECT,no-resolve
  - RULE-SET,cncidr,DIRECT,no-resolve
  - RULE-SET,China,DIRECT,no-resolve
  - RULE-SET,lancidr,DIRECT,no-resolve
  - RULE-SET,collection,DIRECT,no-resolve

  - GEOSITE,geolocation-cn,DIRECT
  - MATCH,低延迟
```

## 配置V2ray落地代理

此步骤与上一步配置Clash分流与链式代理独立，指的是不使用Clash，仅通过V2ray使用家宽代理

V2ray不支持分流，即所有被代理流量（包括需要大带宽的视频，低延迟的游戏等）都会通过家宽代理，计入每月250GB的额度且美国延迟200+ms，若无特殊需求建议参考上方Clash配置教程

点击展开V2ray具体配置教程

本节演示的软件为[v2rayN](https://github.com/2dust/v2rayN)

首先点击左上角服务器-添加SOCKS服务器，并将自己购买的ip端口用户名密码填入，别名填webshare（可以自定义，后续会用到），右上角协议应该无所谓我填的sing\_box

[![添加SOCKS服务器](https://cdn3.linux.do/original/4X/e/5/d/e5ddc09344691d68f5e3b7db8513d6cca8ad3392.png)

添加SOCKS服务器342×483 12.5 KB

](https://cdn3.linux.do/original/4X/e/5/d/e5ddc09344691d68f5e3b7db8513d6cca8ad3392.png "添加SOCKS服务器")

  

[![SOCKS服务器信息](https://cdn3.linux.do/original/4X/a/a/d/aad30d3fba8a60d401671ff91c36dd78bf09112e.png)

SOCKS服务器信息1073×411 6.49 KB

](https://cdn3.linux.do/original/4X/a/a/d/aad30d3fba8a60d401671ff91c36dd78bf09112e.png "SOCKS服务器信息")

然后在订阅设置中点开你自己在用的订阅分组的设置，在落地代理别名填入webshare

[![订阅设置](https://cdn3.linux.do/optimized/4X/a/3/7/a37f029b0c2daf020991dc2928fc3f352f7241de_2_500x500.png)

订阅设置877×876 27.7 KB

](https://cdn3.linux.do/original/4X/a/3/7/a37f029b0c2daf020991dc2928fc3f352f7241de.png "订阅设置")

保存后更新一次订阅，并点击上方重启服务

[![重启服务](https://cdn3.linux.do/original/4X/0/b/9/0b939d679f7d0768bc0a188a8efccb27f97075ae.png)

重启服务592×118 5.69 KB

](https://cdn3.linux.do/original/4X/0/b/9/0b939d679f7d0768bc0a188a8efccb27f97075ae.png "重启服务")

配置完成后可以打开代理访问国外ip测试网站检测是否为家宽ip

## 单月订阅转换包年

如果买了一个月感觉不错，可以把自己的订阅更新为包年订阅，当然也可以等第一个月用完了再重新买包年

在订阅的还未用完的条件下，可以直接按照购买流程重新选中一次，并勾选包年，原始的优惠价格是8美元或9.6美元，下方的Account Credits就是此前订阅中购买后还未使用的余额，余额是按天扣费的（每天约0.03美元），可以直接抵扣

[![包年订阅](https://cdn3.linux.do/optimized/4X/7/2/e/72eeb5659879cc59bf3a3229b2d622486670b73c_2_371x500.png)

包年订阅502×675 22.3 KB

](https://cdn3.linux.do/original/4X/7/2/e/72eeb5659879cc59bf3a3229b2d622486670b73c.png "包年订阅")

# 关于ChatGPT降智的一些观测

ip只是ChatGPT降智的部分因素，目测与账号、使用频率等多个方面都有关

我买的这个家宽代理共有2个人，一共4-5个号在用，我的大号可能因为用的最多，是最容易降智的，即使用了家宽代理有时候提问次数多了也会降，还可能前一天一直不降，第二天第一个问题就降智，此时同同一个代理其他不常用小号是正常的。前几天还遇到了当天前两次正常推理，同一个上下文第三次推理就降智了

用家宽只能尽可能减少降智概率，如果降了可以尝试换ip，频繁更换还是降的话建议直接换号，反正现在注册也不需要验证码，把一个号放几天不用说不定就不降了