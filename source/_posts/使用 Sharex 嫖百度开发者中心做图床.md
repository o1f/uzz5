---
title: 使用 Sharex 嫖百度开发者中心做图床
categories:
  - - Win
tags:
  - Sharex
  - 图床
  - 白嫖
  - 经验
id: '10'
thumbnail: 'https://cdn.uzz5.com/imgs/2021/02/27/to2MrSbj.webp'
abbrlink: j625
date: 2020-12-13 00:17:32
---
因 百度开发者中心 改版,本文已失效,仅做经验分享

## 前言

之前介绍过使用百度贴吧做图床,速度快,也解决了水印问题,但是`https`有防盗链,只有`http`可以用. 没有小绿锁了,没得逼格了.

## 开整

### 抓包

先抓包,跟之前一样 访问[百度开发者中心](https://developer.baidu.com/) ![打开编辑器](https://cdn.uzz5.com/imgs/2021/02/27/j8NhmIwB.webp "打开编辑器") 然后呼出控制栏,点击上传图片查看 ![](https://cdn.uzz5.com/imgs/2021/02/27/v11fQSw4.webp) ![](https://cdn.uzz5.com/imgs/2021/02/27/i3KA8Ibl.webp)

### Sharex 配置

```json
{
  "Version": "13.1.0",
  "DestinationType": "ImageUploader",
  "RequestMethod": "POST",
  "RequestURL": "https://developer.baidu.com/upload/image",
  "Headers": {
    "cookie": "改成你自己的cookie"
  },
  "Body": "MultipartFormData",
  "Arguments": {
    "name": "img",
    "filename": "$filename$"
  },
  "FileFormName": "img",
  "URL": "$json:data.imageUrl$"
}
```

如何使用呢~ 复制以上代码,复制,打开自定义上传,导入,复制剪贴板,修改你的`cookie` ![](https://cdn.uzz5.com/imgs/2021/02/27/hRuZ7yWI.webp)

## 优缺点

### 优点

就一个字 `快`

### 缺点

限制大小 `4M` ,太小了,影响我搞黄色... ![我也想跟你们分享啊~](https://cdn.uzz5.com/imgs/2021/02/27/JMuGWcPf.webp "我也想跟你们分享啊~") 参考原新浪图床

*   可能会防盗链
*   图片审查

## 推荐图床

路过图床:[https://imgchr.com/](https://imgchr.com/) 

LOL图床:[https://imagelol.com/](https://imagelol.com/) (打钱!) 

当然最推荐还是自建,没有什么比数据放到自己手上更安心了. 各大云服务商的云储存服务,以及推荐一下图床源码

*   `cheverto`
*   `Hidove`

下面几款开源的

 - [https://github.com/helloxz/imgurl](https://github.com/helloxz/imgurl) 
 - [https://github.com/wisp-x/lsky-pro](https://github.com/wisp-x/lsky-pro) 
 - [https://github.com/aimerforreimu/auxpi](https://github.com/aimerforreimu/auxpi) 
 - [https://github.com/Hello-hao/Tbed](https://github.com/Hello-hao/Tbed) 
 - [https://github.com/xiebruce/PicUploader](https://github.com/xiebruce/PicUploader)

## 产考

[https://www.hostloc.com/search.php?kw=图床程序](https://www.hostloc.com/search.php?mod=forum&searchid=3485&orderby=lastpost&ascdesc=desc&searchsubmit=yes&kw=%E5%9B%BE%E5%BA%8A%E7%A8%8B%E5%BA%8F) 

[https://www.hostloc.com/thread-673106-1-1.html](https://www.hostloc.com/thread-673106-1-1.html) [https://github.com/](https://github.com/)