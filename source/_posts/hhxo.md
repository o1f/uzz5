---
title: 文章名
date: 时间
categories:
  - - Web
tags:
  - Blog
  - Github
  - hexo
  - 分享
id: '306'
thumbnail:
---


昨天心血来潮想折腾一下 Hexo , 就想起了之前的一个项目, 可以配合下面教程,在线编辑发布文章,不需要在本地构建环境. 这是我根据 本文教程以及 hexoplusplus 创建的 Hexo 个人博客 [https://bref.life](https://bref.life) 原先的 wordpress 可以备份一下删掉了. Hexo 后端开源地址: [https://github.com/HexoPlusPlus/HexoPlusPlus](https://github.com/HexoPlusPlus/HexoPlusPlus)

## 前言

> 本文不适合 需要开发 Hexo 主题、插件 的同学和大佬们阅读。

大部分的 Hexo 教程都会让你安装 Node.js , Git , Hexo 命令行 等工具，而安装这些工具可能会遇到许多问题，抬高了搭建博客的门槛。

其实我们可以利用 Vercel 这一平台搭建，不用敲一行命令，不安装一个程序，用一个浏览器就可完成。

## 你需要准备

*   浏览器
    
*   GitHub 账号（主邮箱不要是 QQ 等邮箱，可能会注册不了 Vercel）
    

## 开始

### 创建 Vercel 账号

使用浏览器访问：[https://vercel.com/signup](https://vercel.com/signup)

点击「Cotinue with GitHub」并使用 GitHub 账号授权登录。

![注册 Vercel 账号](https://cdn.uzz5.com/imgs/2021/03/16/AP42V1oE.webp)

### 从模板新建项目

[点击这里](https://vercel.com/new/git/external?repository-url=https://github.com/oCoke/hexo-template/tree/master) 从模板创建一个 Hexo 应用，名称随意，输入完毕后点击「Continue」。

> Vercel 自带的版本为 3.9.0。
> 
> 此应用将 Hexo 版本更新到了最新（5.3.0），避免了很多错误和问题的发生。

点击 GitHub 标签，输入你导入后的仓库名称（可随意），输入完毕点击「Continue」。![导入至 GitHub 仓库](https://cdn.uzz5.com/imgs/2021/03/16/FrvgNz9w.webp)

可以看到 Vercel 已经自动识别出仓库是 Hexo 框架，点击「Deploy」。

> Project Name 可以随意填写，但必须是唯一的。

![部署博客](https://cdn.uzz5.com/imgs/2021/03/16/8iRxQP7X.webp)

随后 Vercel 就会开始部署，稍等片刻。

部署完毕后，Vercel 会撒花 🎉 庆祝。这时，点击页面中的「Visit」就可以访问站点了。

## 进阶

### 自定义主题

首先，前往 [Hexo 主题列表](https://hexo.io/themes) 找到你喜欢的主题。

点击主题的名称就可以进入到主题的 GitHub 地址。

点击侧边栏中的 Release 进入到最新的发行版下载地址。

没有的话就阅读主题的 README 寻找答案，一般情况下都是有的。

![Release](https://cdn.uzz5.com/imgs/2021/03/16/c4nU4Cdz.webp)

滑动到页面底部，下载文件。你可以选择 .zip 压缩版本或是 .tar.gz 压缩版本。（解压后文件都一样）

![下载发行版](https://cdn.uzz5.com/imgs/2021/03/16/4uLA0a34.webp)

解压下载下来的文件。

访问 [https://vercel.com/dashboard](https://vercel.com/dashboard) ，找到并点击 你部署的博客项目的 卡片。

点击 图片中箭头指的位置 ，进入 GitHub 仓库。

![点击仓库名](https://cdn.uzz5.com/imgs/2021/03/16/t7Kxbkkm.webp)

点击文件区域的 `themes` 目录。

![进入 themes 目录](https://cdn.uzz5.com/imgs/2021/03/16/OlHt26qv.webp)

点击 「Add File」、「Upload Files」上传文件。

![上传文件](https://cdn.uzz5.com/imgs/2021/03/16/va9F23ih.webp)

![拖拽文件](https://cdn.uzz5.com/imgs/2021/03/16/FShnmXAB.webp)

![提交更改](https://cdn.uzz5.com/imgs/2021/03/16/30gPrdSn.webp)

> 提交之后需要稍等一下。

> 如果主题的文件大于 50 个，就无法直接上传。你需要：
> 
> 1.  下载 Git 工具
>     
> 2.  使用 `git clone` 命令将仓库克隆至本地。
>     
> 3.  将主题文件夹添加至本地博客目录的 `themes` 目录下。
>     
> 4.  `git add`, `git commit`, `git push`。 详细的相关教程请参阅：
>     
> 5.  [https://www.runoob.com/git/git-install-setup.html](https://www.runoob.com/git/git-install-setup.html)
>     
> 6.  [https://www.runoob.com/git/git-clone.html](https://www.runoob.com/git/git-clone.html)
>     
> 7.  [https://www.runoob.com/git/git-add.html](https://www.runoob.com/git/git-add.html)
>     
> 8.  [https://www.runoob.com/git/git-commit.html](https://www.runoob.com/git/git-commit.html)
>     
> 9.  [https://www.runoob.com/git/git-push.html](https://www.runoob.com/git/git-push.html)
>     
> 10.  或者使用 Github Desktop
>     

然后记住上传后的文件夹的名字，例如我这里是`oranges`。

返回仓库首页，找到并点击文件区域的 `_config.yml` 文件。

点击修改按钮修改文件：

![修改文件](https://cdn.uzz5.com/imgs/2021/03/16/n6lGe1gF.webp)

修改启用的主题为刚刚上传的主题：

等待 Vercel 自动部署完毕即可。

### 安装插件

首先，进入到 插件 的 GitHub 地址。

找到并点击插件文件区域的 `package.json`，找到 `dependencies` 一项。

复制这几项到博客 `package.json` 文件的 `dependencies` 项中，重复的就不用了。

然后再加入一项，键是 插件名，值是 `^+插件最新版本号`

例如，我要安装 2.1.0 版本的 `hexo-generator-sitemap` 插件：

我就需要在 `dependencies` 项中 添加以下的字段

 "hexo-util": "^2.1.0",
 "micromatch": "^4.0.2",
 "nunjucks": "^3.1.6",
 "hexo-generator-sitemap": "^2.1.0"

> 不要忘记遵守 JSON 语法格式！具体可以百度一下。

![img](https://cdn.uzz5.com/imgs/2021/03/16/mShDLIUm.webp)

等待 Vercel 自动部署完毕即可。

## 其他

原文: [https://note.yfun.top/p/simply-build-your-hexo-blog/](https://note.yfun.top/p/simply-build-your-hexo-blog/)