---
title: 使 Sharex 支持 Webp 格式
categories:
  - Win
tags:
  - Sharex
  - 图片
  - 分享
  - 经验
thumbnail: 'https://cdn.uzz5.com/imgs/2021/04/16/TZVByuaP.webp'
abbrlink: f782
date: 2021-04-16 18:07:17
---

之前写过一篇文章,简单介绍配合使用`imagemagick`转换成`Webp`格式([原文](https://www.uzz5.com/post/j9hs.html)),今天介绍另一种方法.

<!--more-->

同样的需要外部软件配合

软件下载: https://lanzoui.com/i2gBJo6ew7i

## 配置
首先确保你默认截图格式为`png`,`QQ`默认截图是`png`,`Sharex`自带截图功能需要修改配置

![Png](https://cdn.uzz5.com/imgs/2021/04/16/hyZbFV30.webp)

![首先打开动作设置](https://cdn.uzz5.com/imgs/2021/04/16/oiLXFIQ3.webp)

名称: `png→webp`
文件路径: 选择 `%MyDocuments%\tools\cwebp.exe` 压缩包内的 `cwebp.exe`文件
参数: `-mt -z 9 %input -o %output`
输出扩展名: `webp`
扩展名过滤: `png`
勾选隐藏窗口和删除输入文件(删除输入文件也不可能勾选,会在截图文件夹下生成两个文件,一个`webp`,一个`png`)

![截图后动作](https://cdn.uzz5.com/imgs/2021/04/16/9cPWsMPf.webp)

## 其他

体验下来感觉不错,压缩率尚可,对背景透明的也可以兼容(之前介绍的方法不可以,需要修改参数).
缺点:仅支持`png`,大图转换时间可能会比较久.

参考: https://github.com/ShareX/ShareX/issues/5250