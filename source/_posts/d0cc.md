---
title: 利用某论坛附件做免费图床 ShareX快捷上传存储
date: '2021-4-10 23:26:27'
categories:
  - Other
tags:
  - 分享
  - 经验
  - 图床
abbrlink: d0cc
thumbnail: https://static.uzz5.com/i/2021/04/10/PemiWXMj.webp
---

之前分享的 [使用 Sharex 嫖百度开发者中心做图床](https://www.uzz5.com/j625.html) 因为改版升级已经失效了,水贴用的图床没得了.
今天在其他论坛看到有人分享`sharex`的配置,试了一下,使用阿里云的`OSS`,速度很快.
<!--more-->
不限制文件格式,可以上传`txt`,`webp`等等,只不过文件大小限制为 `5MB`.

## 配置

```json
{
  "Name": "bbs.ldmnq.com",
  "DestinationType": "ImageUploader, FileUploader",
  "RequestType": "POST",
  "RequestURL": "https://bbs.ldmnq.com/api/bbs/upload?dir=topic/attachment",
  "FileFormName": "file",
  "ResponseType": "Text",
  "RegexList": [
    "(https://(.*)\\.([0-9A-Za-z]+))"
  ],
  "URL": "$regex:1,1$"
}
```

![直接复制,自定义导入即可](https://static.uzz5.com/i/2021/04/10/dLbtfmZl.webp)

## 测试

![](https://ldbbs.ldmnq.com/bbs/topic/attachment/2021-4/50e76314-b43b-42b7-bbf9-eb40bd0bfc4f.gif)


## 其他

有效期不确定,我只是用来水贴临时使用,不推荐写文长期使用.

原文: https://bbs.itzmx.com/thread-97729-1-1.html