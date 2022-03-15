---
title: 'TeambitionShare : 挂载Teambition文件 可直链分享 支持网盘和项目文件'
categories:
  - - Web
tags:
  - 开源
  - 网盘
id: '32'
thumbnail: 'https://static.uzz5.com/i/2021/03/01/TNRk2BAK.webp'
abbrlink: azzx
date: 2021-01-26 01:14:44
---


# 开源地址

[https://github.com/FlxSNX/TeambitionShare](https://github.com/FlxSNX/TeambitionShare) 

[项目挂载Demo](http://tbfile.ouoacg.com/) 

[网盘挂载Demo](http://tbfile.ouoacg.com/) 访问密码:123456

# 预览

![](https://static.uzz5.com/i/2021/03/01/PcC82Nu8.webp) ![](https://static.uzz5.com/i/2021/03/01/QIuUOBL1.webp) ![](https://static.uzz5.com/i/2021/03/01/cGhTqXRX.webp)

# 配置环境

*   PHP版本要求 ≥ 5.6
*   PHP版本推荐 ≥ 7.0

# 配置说明

在没有配置文件时访问网站会跳转到配置向导,在配置向导页面填写对应的参数即可生成配置文件 先去 [https://www.teambition.com/](https://www.teambition.com/) 注册登录

## Cookie获取

F12 -> Network -> 刷新一下 找到如图所示的cookie ![](https://static.uzz5.com/i/2021/03/01/aPHlUEpB.webp)

## 项目ID(projectId)获取

先创建一个项目,然后进入创建的项目 ![](https://static.uzz5.com/i/2021/03/01/CzKYXsBk.webp) ![](https://static.uzz5.com/i/2021/03/01/aNh69q31.webp)

## Docker

```shell
docker pull flxsnx/teambitionshare
docker run -d -p 8081:80 flxsnx/teambitionshare:latest
# 访问: http://ip:8081
```

# 伪静态规则

## Nginx

```
# 根目录伪静态
location / {
  if (!-e $request_filename){
    rewrite ^(.*)$ /index.php/?s=$1;
  }
}
# 二级目录伪静态，自行修改pan为你的二级目录名字
location /pan {
  if (!-e $request_filename){
    rewrite ^/pan/(.*)$ /pan/index.php/?s=$1;
  }
}
```

## Apache

```
<IfModule mod_rewrite.c>
  Options +FollowSymlinks -Multiviews
  RewriteEngine On
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteRule ^(.*)$ index.php/?s=$1 [QSA,PT,L]
</IfModule>
```

# 其他

1.  Cookie有效期

目前未遇到cookie失效的情况,猜测只要你不在官网手动退出登录就不会失效

1.  下载速度

下载速度有些不稳定,有时快有时慢(1MB/S);

1.  访问密码

①)全局密码 在config/app.cfg.php中添加 'password' => '你要设置的密码' 即可 ②)目录密码 在目录下上传一个文件.password,文件内容即为目录密码

1.  二级目录运行

放在二级目录运行,配置的时候填入对应的URL和修改伪静态规则(Apache无需修改)即可

# 更多

问题或建议请移步项目地址反馈 [https://github.com/FlxSNX/TeambitionShare](https://github.com/FlxSNX/TeambitionShare) 记得star! ![请输入图片描述](https://static.uzz5.com/i/2021/03/01/Zp9ru19H.webp "请输入图片描述")