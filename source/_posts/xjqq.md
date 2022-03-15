---
title: 'Debian/Ubuntu/CentOS 网络安装/网络重装/纯净安装 一键脚本'
date: 2020-12-13 19:21:27
categories:
  - - Other
tags:
  - Github
  - Linux
id: '5'
thumbnail: https://static.uzz5.com/i/2021/02/27/RRsAYTrZ.webp
abbrlink: xjqq
---


## 起始

在大佬那里买了`AWS`,首选的时候没发现默认系统更改了,买成了 `Ubuntu`,由于习惯了`centos`,想要`DD`重装一下.

> 关键`Centos`宝塔兼容好...

## 介绍

用到了 `Vicer` 萌咖大佬的脚本，感谢~

### 支持重装的系统：

*   Debian 9/10
*   Ubuntu 18.04/16.04
*   CentOS 6/7
*   自定义DD镜像

### 特性/优化：

*   自动获取IP地址、网关、子网掩码
*   自动判断网络环境，选择国内/外镜像，再也不用担心卡半天了
*   超级懒人一键化，无需复杂的命令
*   解决萌咖脚本中一些导致安装错误的问题
*   `CentOS 7` 镜像抛弃`LVM`，回归`ext4`，减少不稳定因素

## 使用方法

```
wget --no-check-certificate -O AutoReinstall.sh https://git.io/AutoReinstall.sh && bash AutoReinstall.sh
```

## 预览

![](https://static.uzz5.com/i/2021/02/27/kV0wqJGW.webp)

## 其他

记得修改默认密码! 我使用的是`AWS`,重装的`centos`,执行之后,大概会失联十几分钟,简单快捷. 唯一的缺憾就是,我眼拙,把我做站的机子给重装了.. **关键我还没备份!**

## 引用

原文:[https://www.hostloc.com/thread-645870-1-1.html](https://www.hostloc.com/thread-645870-1-1.html) 

萌咖博客:[https://moeclub.org/](https://moeclub.org/)