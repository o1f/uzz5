---
title: 文章名
date: 时间
categories:
  - - Web
tags:
  - 分享
  - 开发
  - 白嫖
  - 经验
id: '67'
thumbnail:
---


本文系转载,原文地址： [https://www.jingtaiboke.com/unicloud-upload-demo.html](https://www.jingtaiboke.com/unicloud-upload-demo.html) 问题，建议及反馈请前往原文留言讨论。 根据原文所介绍，dcloud 的用处可不仅仅是做图床文件外链那么简单了，希望各位开发者好好利用，而不是滥用。 本博客不推荐做长期文件储存来用的，数据不保证，无法有效备份。（还不如GitHub+jsd，可以定时任务进行备份，单文件20M对于图片以及静态资源够用了） 疑似开发者在原文中的回应 ![请输入图片描述](https://cdn.uzz5.com/imgs/2021/02/28/j6X0J1VZ.webp "请输入图片描述") 以下为原文：

> 本文将从零部署一个基于阿里云免费cnd的文件上传程序,演示整个部署过程以及一些坑

## 效果演示

[演示（仅作演示，不定期关闭）](https://static-72b0ccd4-7020-4f7c-bebc-1099f822e2bc.bspapp.com/#/)

## 准备工作

## 账号注册,以及实名认证

[https://unicloud.dcloud.net.cn/home](https://unicloud.dcloud.net.cn/home)

## 演示源码下载

[下载：（密码2233）](https://545c.com/d/19473836-42522931-e58c84) 下载后解压

## 开发环境下载

绿色软件,解压直接运行 请选 [App开发版（261.97M）](https://download1.dcloud.net.cn/download/HBuilderX.3.1.2.20210206.full.zip),不要那个小的

## 用编辑器打开源码

Ctrl+O,选择源码文件夹

## 开始部署

现在你的界面应该是这样的 ![请输入图片描述](https://cdn.uzz5.com/imgs/2021/02/28/JxlxStmX.webp "请输入图片描述")

## 创建云服务空间

右键`uniCloud`文件夹,选择创建云服务空间,选阿里云

## 关联云服务空间

右键`uniCloud`文件夹,选择关联云服务空间,选刚才创建的

## 开通前端托管

*   web端,进入刚才创建的空间,点击”前端网页托管”,
*   再点`开通`,稍等几秒钟
*   点`参数配置`,复制`默认域名`
    
    > 例如`static-02198a5f-6b42-463e-844f-acd44036e817.bspapp.com`
    
*   再点跨域配置,将刚才的默认域名加上,当然你可以绑定自己的备案域名
    
    > 这一步很重要,否则云函数不会执行
    

![请输入图片描述](https://cdn.uzz5.com/imgs/2021/02/28/QqYS6YNy.webp "请输入图片描述") ![请输入图片描述](https://cdn.uzz5.com/imgs/2021/02/28/U1q7bk4L.webp "请输入图片描述")

## 上传部署

进入编辑器,选中左侧项目–\\> 点菜单`发行` –\\> 点`上传网站到服务器` 稍等片提示成功,竣工 ![请输入图片描述](https://cdn.uzz5.com/imgs/2021/02/28/H09kPuSk.webp "请输入图片描述")

## unicloud的实际应用

[静态博客编辑器](https://jingtaiboke.com/),是一个静态博客管理后台. 已经融合unicloud阿里云图片上传,使用方法很简单

> 截图 –\\> Ctrl+V 直接插入到文章中 右键复制网页图片 –\\> Ctrl+V 也是支持的

从此写静态博客又方便了不少 ![请输入图片描述](https://cdn.uzz5.com/imgs/2021/02/28/32Yww6xs.webp "请输入图片描述")