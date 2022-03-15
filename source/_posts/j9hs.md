---
title: Sharex 截图压缩并转换成 webp格式
categories:
  - - Win
tags:
  - 工具
  - 经验
id: '9'
thumbnail: 'https://static.uzz5.com/i/2021/02/27/gSunC711.webp'
abbrlink: j9hs
date: 2021-02-21 00:15:40
---


## webp 兼容

[https://caniuse.com/?search=webp](https://caniuse.com/?search=webp) ![](https://static.uzz5.com/i/2021/02/27/OfeeuO5R.webp) 谷歌家推出的,所以说基本上全线产品支持,`chrouim` 系列浏览器就不多说了. `firefox`64以上版本也支持,现阶段就`ios`不支持了 .对于我来说问题不大,我又没有苹果手机了.也没得`ipad` 

* * *

我一直在使用`Sharex`,这款软件真的是功能太强大了,有兴趣的朋友可以百度一下,很多人有写,我就不再东施效颦了. 推荐阅读 [https://www.baidu.com/s?ie=UTF-8&wd=sharex](https://www.baidu.com/s?ie=UTF-8&wd=sharex)

## 图片压缩

我现在使用的图床是 `github`+`jsdelivr`,加载速度很快,但俗话说的好啊,越快越好嘛,所以想到了压缩. 然后就发现了`webp`格式,高效,,兼容,压缩率高,所以说嘛折腾一下~ 由于本人不是一个技术流,例行惯例,百度一下.

## sharex + imagemagick

`sharex` 是支持命令行处理的,`imagemagick`是可以命令行处理的~ so..

## 经验分享

### 下载 imagemagick

官网:[https://imagemagick.org/script/download.php](https://imagemagick.org/script/download.php) (`win`版本在下面)

### 下载 file2clip.exe

`file2clip` 是用来监控文件并复制到剪贴板,方便使用快捷键上传,开源工具 

直接下载: [https://raw.sevencdn.com/rostok/file2clip/master/file2clip.exe](https://raw.sevencdn.com/rostok/file2clip/master/file2clip.exe) 

开源地址:[https://github.com/rostok/file2clip](https://github.com/rostok/file2clip)

## 动作设置

### 动作设置位置

![](https://static.uzz5.com/i/2021/02/27/VCbb3IlW.webp)

### imagemagick

先添加 `imagemagick`动作 ![](https://static.uzz5.com/i/2021/02/27/zAXAYgIv.webp) 名称随意,路径选择`magick.exe`执行路径,例如`E:\Program Files\ImageMagick-7.0.10-Q16\magick.exe` 参数:

```json
clipboard: -strip -interlace Plane -sampling-factor 4:2:0  -quality 75% clipboard: "F:\Documents\ShareX\Screenshots\temp.webp"
```

`F:\Documents\ShareX\Screenshots\temp.webp` 自行修改存储位置 下面最好勾上隐藏窗口. 确定保存.

> 参数我照抄的,自己可以看一下文档个性化一下~

### file2clip

![](https://static.uzz5.com/i/2021/02/27/dA5PfhIc.webp) 名称随意,路径与`imagemagick`相似,为执行文件路径 参数就填写你刚才`imagemagick`设置存储`webp`的路径. 下面的隐藏窗口记得点,要不然截图之后会有窗口一闪而过...

### 其他设置

保持之后勾选两个动作,之前有一个默认的记得取消 . ![](https://static.uzz5.com/i/2021/02/27/1S5Vp6lv.webp) ![然后设置截图之后行为](https://static.uzz5.com/i/2021/02/27/OE0QYpOL.webp "然后设置截图之后行为")

## 图片对比

![原图](https://static.uzz5.com/i/2021/02/27/EWDlTxOR.jpg "原图") ![属性](https://static.uzz5.com/i/2021/02/27/AL3X8jKw.webp "属性")

### 压缩之后

![图片](https://static.uzz5.com/i/2021/02/27/DvDeY4fY.webp "图片") ![属性](https://static.uzz5.com/i/2021/02/27/S58dL9rW.webp "属性")

## 其他

压缩肯定会损害图片质量,这个大家可以调整参数,更改成适合自己的. 另外其他软件截的图,或者本地图片,可以使用`Shrex`自带的图片编辑器,打开之后保存就可以生成`webp`文件了. 录制的`gif`图片暂时无法转换格式,

推荐使用： [https://renzhezhilu.gitee.io/webp2jpg-online/](https://renzhezhilu.gitee.io/webp2jpg-online/) 

其他方式：Png → webp ୧(๑•̀⌄•́๑)૭ [https://github.com/ShareX/ShareX/issues/5250](https://github.com/ShareX/ShareX/issues/5250)

## 引用

原文:[https://bbs.saraba1st.com/2b/thread-1921455-1-1.html](https://bbs.saraba1st.com/2b/thread-1921455-1-1.html) 

参考:[https://capriccio.moe/archives/60/](https://capriccio.moe/archives/60/)