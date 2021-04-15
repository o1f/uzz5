---
title: '[开源] 基于 CF Worker KV 的短链接/短网址程序'
date: 2020-12-15 20:00:07
categories:
  - - Web
tags:
  - Github
  - 开源
id: '17'
thumbnail: https://cdn.uzz5.com/imgs/2021/02/28/Rpg52giJ.webp
abbrlink: 20uh
---


很多时候网址过长不利于分享，将长网址转换短网址/短链接，缩短内容长度，会使得分享更加方便。 借助免费的 `Cloudflare Worker` 和前不久新添加的kv免费额度可以搭建属于我们自己的长网址转换短网址程序

# 开源地址

开源地址: [https://github.com/xyTom/Url-Shorten-Worker](https://github.com/xyTom/Url-Shorten-Worker)

# demo 地址

[https://5it.me](https://5it.me)

# 使用方法

首先去 [https://workers.cloudflare.com/](https://workers.cloudflare.com/) 注册一个账号 

去 `Workers KV` 中创建一个命名空间 ![](https://cdn.uzz5.com/imgs/2021/02/28/K8FegBmx.webp) 

去`Worker`的`Settings`选选项卡中绑定`KV Namespace` ![](https://cdn.uzz5.com/imgs/2021/02/28/BYELjQFc.webp) 

复制本项目中的`index.js`的代码到 `Cloudlare Worker` 点击 `Save and Deploy`

# 演示

![](https://cdn.uzz5.com/imgs/2021/02/28/QVfEUSXR.webp)

# 其他

缺点: 无后台,无法管理查看数据,`KV`有免费额度限制，每天只能写`1000`次 优点: 方便,免费,无需服务器. ![](https://cdn.uzz5.com/imgs/2021/02/28/rTqvkNQQ.webp)

# 其他+

本文系转载,原文链接:[https://www.hostloc.com/thread-778383-1-1.html](https://www.hostloc.com/thread-778383-1-1.html)