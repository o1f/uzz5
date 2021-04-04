---
title: '镜像加速解决国内服务器拉去 Docker 镜像速度慢/失败的方法'
date: 2021-3-7 19:01:58
categories:
  - - Other
tags:
  - docker
  - 分享
  - 工具
  - 开发
  - 阿里云
id: '265'
thumbnail: https://cdn.uzz5.com/imgs/2021/03/10/EYAFYGDB.webp
---


今天使用宝塔 Docker 部署 [ArchiSteamFarm](https://github.com/JustArchiNET/ArchiSteamFarm) 的时候,拉取镜像的时候等了好久,没成功,就百度,看到有镜像加速就百度了一下,记录方便以后使用.

## 国内加速地址

类别

地址

Docker官方中国区设定

[https://registry.docker-cn.com](https://registry.docker-cn.com)

ustc

[https://docker.mirrors.ustc.edu.cn](https://docker.mirrors.ustc.edu.cn)

网易

[http://hub-mirror.c.163.com](http://hub-mirror.c.163.com)

阿里云

需要开发者账号：阿里云开发平台->Docker镜像仓库->加速器（开发者专属，一般格式为[https://xxxxx.mirror.aliyuncs.com](https://xxxxx.mirror.aliyuncs.com)）

## 阿里云链接

登陆地址: ([https://cr.console.aliyun.com](https://cr.console.aliyun.com)) ![](https://cdn.uzz5.com/imgs/2021/03/07/VMSS06ek.webp) 创建一个镜像仓库 ![](https://cdn.uzz5.com/imgs/2021/03/07/jjAoZXDd.webp) 选择本地仓库即可 ![](https://cdn.uzz5.com/imgs/2021/03/07/vMjdKztr.webp) 获取加速地址

## 宝塔 Docker

![](https://cdn.uzz5.com/imgs/2021/03/07/uy5dME6p.webp)

## SSH 终端

在终端依次输入

```shell
sudo mkdir -p /etc/docker 
sudo tee /etc/docker/daemon.json <<-'EOF'
 {  
"registry-mirrors": \["你的加速地址"\]
 } 
EOF 
sudo systemctl daemon-reload //重新加载 
sudo systemctl restart docker //重启Docker
```

![](https://cdn.uzz5.com/imgs/2021/03/07/9HcPn8zn.webp) 也可以直接使用 Vim 编辑 /etc/docker/daemon.json

```shell
vim /etc/docker/daemon.json
```

## Mac 与 Windows

可查看阿里云镜像服务操作文档 ![](https://cdn.uzz5.com/imgs/2021/03/07/HGoiTUv8.webp)

## 其他

### 参考链接

*   [下载镜像太慢的解决方案](https://www.jb51.net/article/206785.htm)
    
*   [docker镜像加速设定方式](https://blog.csdn.net/liumiaocn/article/details/87606919)