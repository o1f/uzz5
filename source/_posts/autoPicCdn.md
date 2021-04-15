---
title: 'autoPicCdn: 基于 Github + Jsdelivr 的简洁图床程序'
categories:
  - - Web
tags:
  - Github
  - 图床
  - 开源
id: '48'
thumbnail: 'https://cdn.uzz5.com/imgs/2021/02/28/0I3nJyHV.webp'
abbrlink: 3lrw
date: 2021-01-28 01:27:10
---


开源地址: [https://github.com/yumusb/autoPicCdn](https://github.com/yumusb/autoPicCdn) 演示地址: [https://piegun.com/](https://piegun.com/)

# 预览

![](https://cdn.uzz5.com/imgs/2021/02/28/iJgPpnGu.webp)

# 其他

分享一个 sharex 配置 ,sharex 是什么百度一下,强大的截图处理工具

```
{
  "Version": "13.1.0",
  "DestinationType": "ImageUploader",
  "RequestMethod": "POST",
  "RequestURL": "域名/up.php",
  "Body": "MultipartFormData",
  "FileFormName": "pic",
  "URL": "$json:data.url$"
}
```

![](https://cdn.uzz5.com/imgs/2021/02/28/ZFwiIYkS.webp)

# 其他

部署及其他说明请查看开源项目说明. 作者上线了两个线上版本,无须自己部署,只需要设置仓库信息即可.

## 线上版本：

*   [https://chuibi.cn/](https://chuibi.cn/)支持Github的在线上传与API接口。通过github授权登录并设置仓库等信息后可用。
*   [https://chuibi.net/](https://chuibi.net/)支持Gitee的在线上传与API接口。通过gitee授权登录并设置仓库等信息后可用。