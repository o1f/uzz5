---
title: 'webp2jpg-online：使用浏览器的在线图片格式转化器'
date: 2021-1-23 19:46:53
categories:
  - - Web
tags:
  - 图片
  - 工具
id: '36'
thumbnail: https://cdn.uzz5.com/imgs/2021/02/28/aYGUCT6a.webp
abbrlink: zu8h
---


![请输入图片描述](https://cdn.uzz5.com/imgs/2021/02/28/jtxXhpsb.webp "请输入图片描述")

# 项目地址

[GitHub](https://github.com/renzhezhilu/webp2jpg-online) 

[Web](https://renzhezhilu.github.io/webp2jpg-online)

# 预览

![请输入图片描述](https://cdn.uzz5.com/imgs/2021/02/28/HBCAitmp.webp "请输入图片描述")

# 功能特点

- 无需上传，使用浏览器自身进行转换 
- 批量转换输出 WebP、JPEG、PNG、Base64、8位 PNG（实验）、GIF 动图（实验）、WebP 动图（实验） 
- 输出指定大小（WebP、JPEG）（实验） 
- 输出颜色数量（GIF、PNG-8) - 选项可自定增加或删除并持久化 
- 无需上传图片至远端服务器，本地完成转换 

本项目主要利用 HTML5 自带的接口 HTMLCanvasElement.toBlob()，在本地完成图片格式转换，主打「简单、隐私」。这一点和其他在线图片格式转换与压缩站点有所不同，其他方面中规中矩 试了一下，处理的速度很快，压缩和转换的效果也不错，这里大家自行去测试。比较遗憾的就是他们的前后压缩「对比」功能，即使拉到最大也看不真切，建议大家安装浏览器插件 Imagus 等进行光标停滞放大。此外，WebP 动画、PNG、GIF 转换下，图片有一定概率会出现错误，本工具也不支持无损转换 当然，大家也可以通过 ImageMagick、ImageOptim 等工具完成图片格式的转换

# 其他

本文系转载,原文:[https://t.me/NewlearnerChannel/5340](https://t.me/NewlearnerChannel/5340) 

问题及建议请移步:[https://github.com/renzhezhilu/webp2jpg-online/issues](https://github.com/renzhezhilu/webp2jpg-online/issues)