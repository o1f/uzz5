---
title: 'lsky-pro: 免费简洁但功能强大，支持多家对象储存的图床程序'
date: 2021-4-22 19:33:26
categories:
  - Web
tags:
  - 图床
  - 开源
  - Github
thumbnail: https://static.uzz5.com/i/2021/04/22/ibGDZUxU.webp
abbrlink: v5za
---

> Your photo album on the cloud.

[开源地址](https://github.com/wisp-x/lsky-pro/)|[详细文档](https://www.kancloud.cn/wispx/lsky-pro)|[演示Demo](https://pic.iqy.ink/)|[浏览器扩展](https://github.com/wisp-x/lsky-pro-chrome-extension)

[下载地址](https://github.com/wisp-x/lsky-pro/releases)|[问题建议](https://github.com/wisp-x/lsky-pro/issues)|[TG群组](https://t.me/lsky_pro)

## 预览

![](https://static.uzz5.com/i/2021/04/22/btlVQobq.webp)
![](https://static.uzz5.com/i/2021/04/22/ycZWnXVo.webp)

## 特点

* [x] 支持第三方云储存，本地、阿里云 OSS、腾讯云 COS、七牛云、又拍云、FTP
* [x] 多图上传、拖拽上传、粘贴上传、上传预览、全屏预览、页面响应式布局
* [x] 简洁的图片管理功能，支持鼠标右键、单选多选、重命名等操作
* [x] 全局配置用户初始剩余储存空间、设置指定用户剩余储存空间
* [x] 一键复制图片外链、二维码扫描链接、图片鉴黄功能
* [x] 设置上传文件、文件夹路径命名规则、文件夹分类功能
* [x] 接口上传、图片软删除
* [x] OTA 在线升级系统
* [x] (Dark)暗黑主题
* [x] IP 封禁功能(支持通配符)
* [x] 自定义链接参数
* [x] 单用户模式
* [x] 图片广场(画廊)
* [x] 上传图片自动增加水印(支持图片或文字)

## 安装要求
* PHP 版本 &ge; 5.6
* mysql 版本 &ge; 5.5
* PDO 拓展
* ZipArchive 支持
* fileinfo 拓展
* curl 拓展

注：如果使用 FTP 功能，需要开启 PHP 的 FTP 拓展

## 安装教程
1. 下载兰空，上传至 web 运行环境，解压。
2. 设置运行目录为 public。
3. 配置 Rewrite 规则：
    ##### Nginx：
    ```
    location / {
        if (!-e $request_filename) {
        	rewrite ^(.*)$ /index.php?s=$1 last; break;
        }
    }
    ```

    ##### Apache:
    Apache 直接使用 .htaccess 即可

4. 访问首页，未安装自动跳转至安装页面，根据页面提示安装即可。
5. 安装完成以后请设置 runtime 目录 0755 权限，如果你使用本地存储，public 目录也需要设置为 0755 权限

