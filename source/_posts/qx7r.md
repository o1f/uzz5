---
title: 人手一个博客之——运行在 cloudflare workers 的博客
categories:
  - - Web
tags:
  - Blog
  - Coudflare
  - Github
id: '23'
thumbnail: 'https://static.uzz5.com/i/2021/02/28/FcWzIFuL.webp'
abbrlink: qx7r
date: 2020-12-23 23:42:03
---


一个运行在 `cloudflare workers` 的博客 `blog`，使用 `KV` 数据库存储数据,`cloudflare` 给了`1G` 的 `KV` 数据库,完全够用了~ 静态博客的原理，动态博客的管理后台，发布文章快捷方便 更关键的，他完全免费!

# 开源项目

[https://github.com/gdtool/cloudflare-workers-blog](https://github.com/gdtool/cloudflare-workers-blog) 

Demo演示: [https://blog.gezhong.vip/](https://blog.gezhong.vip/)

# 主要特点

*   使用workers提供的KV作为数据库
*   使用cloudflare缓存html来降低KV的读写
*   所有html页面均为缓存,可达到静态博客的速度
*   使用KV作为数据库,可达到wordpress的灵活性
*   后台使用markdown语法,方便快捷
*   一键发布(页面重构+缓存清理)

# 承载能力

*   KV基本不存在瓶颈,因为使用了缓存,读写很少
*   唯一瓶颈是 workers的日访问量10w,大约能承受2万IP /日
*   文章数:1G存储空间,几万篇问题不大

# 部署及应用

访问 [https://blog.gezhong.vip/](https://blog.gezhong.vip/) 查看具体使用事宜.

# 预览

![](https://static.uzz5.com/i/2021/02/28/amkrfTV7.webp ) ![](https://static.uzz5.com/i/2021/02/28/ChnLGn5C.webp )

# 参考

来源:[https://www.hostloc.com/thread-787159-1-1.html](https://www.hostloc.com/thread-787159-1-1.html) 

开源地址:[https://github.com/gdtool/cloudflare-workers-blog](https://github.com/gdtool/cloudflare-workers-blog) 

Demo演示&教程说明:[https://blog.gezhong.vip](https://blog.gezhong.vip)