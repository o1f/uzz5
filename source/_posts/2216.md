---
title: 'Video_spider: 短视频/图集在线去水印解析'
categories:
  - Web
tags:
  - Github
  - 开源
  - 工具
thumbnail: 'https://cdn.uzz5.com/imgs/2021/04/11/byTrztjv.webp'
abbrlink: '2216'
date: 2021-04-11 12:45:23
---

短视频去水印：抖音/皮皮虾/火山/微视/微博/绿洲/最右/轻视频/`instagram`/哔哩哔哩/快手/全民小视频/皮皮搞笑/全民k歌/巴塞电影/陌陌/`Before`避风/开眼/Vue Vlog/小咖秀/西瓜视频

<!-- more -->

开源地址: https://github.com/5ime/video_spider

## 预览

[演示网站](https://lab.5ime.cn/video/)

![](https://cdn.uzz5.com/imgs/2021/04/11/4isDdhGL.webp)

## 支持平台

| 平台 | 状态| 平台 | 状态| 平台 | 状态| 平台 | 状态| 平台 | 状态|
|  ----  | ----  | ----  | ---- |----|----|----|----|----|----|
| 皮皮虾 | ✔ | 抖音短视频 | ✔ | 火山短视频 | ✔| 皮皮搞笑 | ✔ | 全民K歌 | ✔ |
| 微视短视频 | ✔ | 微博 | ✔ | 最右 | ✔| vuevlog | ✔ |小咖秀| ✔|
| 轻视频 | ✔ | 快手短视频 | ✔ | 全民小视频 | ✔|陌陌 | ✔ | Before避风 | ✔ | 开眼 | ✔|
| 西瓜视频 | ✔|

## 部署说明

详见开源项目地址,我简单部署了一下.下载代码,上传服务器.

接口地址就是`index.php`所在路径,在根目录即`https://www.xxxx.com/?url=`

然后修改一下示例页面配置
- `demo.html`第`98`行请修改为`你的接口地址`
- `demo.py`第`7`行请修改为`你的接口地址`

![](https://cdn.uzz5.com/imgs/2021/04/11/4FXDgRhF.webp)

如果你只想要托管一个静态网页,而不想自建`API`可以不配置`PHP`环境,直接填写作者的`API`: `https://tenapi.cn/video/?url=`

然后根据自身情况,修改`html`内代码即可.

## 其他

更多详细说明请查看[开源地址](https://github.com/5ime/video_spider),不要忘记`star`哦.

问题建议移步: [issues](https://github.com/5ime/video_spider/issues)

作者还有其他的一些`API`服务,有兴趣可以访问 https://tenapi.cn/ 看一下.