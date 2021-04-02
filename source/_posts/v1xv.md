---
title: 文章名
date: 时间
categories:
  - - Web
tags:
  - Github
  - 图床
  - 工具
  - 开源
id: '274'
thumbnail:
---


我现在正在使用, 之前是利用程序中专上传到 `github` 做图床, 现在是上传到又拍云,因为之前提过建议,使用MD5验证文件,避免重复上传文件,很有用~ 作者反馈特别及时详细,特别推荐,有好的建议或者反馈可直接前往开源地址提 `issues` 一个还不错的图床工具，支持Mac/Win/Linux服务器、支持压缩后上传、添加图片或文字水印、多文件同时上传、同时上传到多个云、右击任意文件上传、快捷键上传剪贴板截图、Web版上传、支持作为Mweb/Typora发布图片接口、作为PicGo/ShareX/uPic等的自定义图床，支持在服务器上部署作为图床接口，支持上传任意格式文件。 开源地址: [https://github.com/xiebruce/PicUploader](https://github.com/xiebruce/PicUploader)

## 主要功能

*   支持Mac和Windows(也可用于Linux服务器端)、理论上也支持Linux桌面版，只要你能添加右键菜单或者用快捷键调用上传命令的话；
*   支持图片压缩后上传(支持jpg/png/webp，gif/bmp不支持压缩)；
*   支持添加水印后上传(支持文字水印、图片水印、自定义水印颜色/透明度/角度/位置，支持jpg/png/bmp/webp，gif不支持水印)；
*   返回的链接可自定义（如原始链接、Markdown格式链接、可点击的Markdown格式链接、完全自定义的链接）；
*   完全自定义上传文件名(可选变量有当前年、月、日、当前时间戳，随机字符串(可调长度))；
*   上传过的文件直接返回历史记录(防止重复上传，仅限在不添加水印不压缩的情况下)；
*   可作为MWeb/Typora的API使用，可作为PicGo/ShareX/uPic等的自定义图床使用；
*   支持快捷键上传剪贴板中的图片(配合Alfred/WinHotKey使用)；
*   支持Web端拖放、粘贴、或直接选择上传图片；
*   支持Web端设置所有参数；
*   支持上传任意格式文件(除了图片，还可以上传任意格式文件，只要你的存储端支持就行)；
*   目前支持的图床：七牛、腾讯、网易、百度、京东、阿里、又拍、sm.ms、Imgur、Ucloud、青云、Nextcloud、Github、Gitee(码云)、Cloudinary、Chevereto、Minio、Aws s3、金山、华为、DropBox、OneDrive、GoogleDrive、Azure、Gitlab、图速云、个人服务器(sftp)、本地(即PicUploader所在机器)。
*   注：之前支持的coding.net由于封了token方式授权的接口，所以现在暂时不支持coding.net。

## 预览

![](https://cdn.uzz5.com/imgs/2021/03/10/UHsjLHd1.webp) ![](https://cdn.uzz5.com/imgs/2021/03/10/PwBNV9YY.webp) ![](https://cdn.uzz5.com/imgs/2021/03/10/zKOX208H.webp)

## 部署

原文档真的是太详细了,包括从 `Mac` 到 `Win` 的全套部署及使用教程,我就简单写一下自己用宝塔部署的过程,以及 `Sharex` 的使用方法.

### 伪静态

首先创建网站,可以使用 `sqlite` 保存数据,也可以使用数据库,看自己需求. 使用 `sqlite` 就不需要创建数据库了 填写伪静态

```shell
    location / {
        index dashboard.php;
        try_files $uri $uri/ index.php$is_args$args;
    }

    location ~ \.php$ {
        fastcgi_index index.php;
        include fastcgi.conf;
    }
```

### 下载程序

推荐 `Git Clone` 方式, 也可以直接下载仓库然后上传 打开终端,或在宝塔面板网站文件夹点击上方 `终端` 输入以下命令,拉取代码

```shell
git clone https://github.com/xiebruce/PicUploader.git .
```

国内服务器推荐使用

```shell
git clone https://github.com.cnpmjs.org/xiebruce/PicUploader.git .
```

更新也只需要执行 `git pull` 即可.

### 配置

接着访问网址即可,我第一次部署的时候有报错,修改文件权限即可 ![](https://cdn.uzz5.com/imgs/2021/03/10/8sOzo3PH.webp) 配置内容较多,但都直观简洁,容易配置,不懂可以留言,我就不写了.

## Sharex

[https://www.xiebruce.top/1095.html#ShareX](https://www.xiebruce.top/1095.html#ShareX) 还是看作者的吧,更详细.

## 其他

反馈建议: [https://github.com/xiebruce/PicUploader/issues](https://github.com/xiebruce/PicUploader/issues) 更多请查看项目文档,或作者博文: [https://www.xiebruce.top/17.html](https://www.xiebruce.top/17.html)