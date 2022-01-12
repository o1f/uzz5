---
title: 简单代码使用视频做博客背景
categories:
  - - Web
tags:
  - Blog
id: '30'
thumbnail: 'https://static.uzz5.com/imgs/2021/03/01/9IXPyauy.webp'
abbrlink: babs
date: 2021-01-03 01:00:06
---


# 示例

https://static.uzz5.com/imgs/2021/03/01/ignK6Dm6.mp4

# 教程

## 添加自定义css

```css
video{  
            position: fixed;  
            right: 0px;  
            bottom: 0px;  
            min-width: 100%;  
            min-height: 100%;  
            height: auto;  
            width: auto;  
            /*加滤镜*/
            /*filter: blur(15px); //背景模糊设置 */
            /*-webkit-filter: grayscale(100%);*/  
            /*filter:grayscale(100%); //背景灰度设置*/  
            z-index:-11
```

## body标签代码

在body标签内添加代码

```html
<video autoplay loop muted>
  <source src="./movie.mp4" type="video/mp4"  />
Your browser does not support the video tag.
</video>
```

`src`后可以是本地文件或者外链,支持格式:`Ogg`、`MPEG4`、`WebM`

# 其他

获取合适的背景视频:[https://keylol.com/t672929-1-1](https://keylol.com/t672929-1-1) 移动端未适配,仅支持pc端,仅供参考,不推荐使用.

# 引用

[https://blog.csdn.net/seanxwq/article/details/80760895](https://blog.csdn.net/seanxwq/article/details/80760895)