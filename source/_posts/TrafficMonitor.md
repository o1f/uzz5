---
title: 'TrafficMonitor: 显示当前网速、CPU及内存利用率的桌面悬浮窗软件'
date: 2021-3-3 19:14:02
categories:
  - - Win
tags:
  - 工具
  - 开源
  - 软件
id: '101'
thumbnail: https://cdn.uzz5.com/imgs/2021/03/03/dJpQSJBi.webp
---


开源地址: [https://github.com/zhongyang219/TrafficMonitor](https://github.com/zhongyang219/TrafficMonitor)

# 简介

Traffic Monitor是一款用于Windows平台的网速监控悬浮窗软件，可以显示当前网速、CPU及内存利用率，支持嵌入到任务栏显示，支持更换皮肤、历史流量统计等功能。

# 相关链接：

请[点击此处](https://github.com/zhongyang219/TrafficMonitor/releases/latest)下载TrafficMonitor的最新版本。 

备用链接：[百度网盘下载](https://pan.baidu.com/s/15PMt7s-ASpyDwtS__4cUhg) 提取码：`ou0m` 

如果遇到问题，请[点击此处](https://github.com/zhongyang219/TrafficMonitor/blob/master/Help.md)

# 主要特性

*   显示当前实现网络传输速率、CPU和内存占用率
*   如果电脑有多个网卡，支持自动和手动选择网络连接
*   查看网络详细信息
*   支持嵌入到任务栏显示
*   支持更换皮肤和自定义皮肤
*   历史流量统计

# 使用说明

**[点击这里](https://github.com/zhongyang219/TrafficMonitor/wiki)转到Wiki页面查看关于TrafficMonitorr的详细说明文档。** 

截图 

主悬浮窗： ![](https://cdn.uzz5.com/imgs/2021/03/03/r51ArDbA.webp) 

右键菜单： ![](https://cdn.uzz5.com/imgs/2021/03/03/C8o09ioV.webp) 

任务栏窗口： ![](https://cdn.uzz5.com/imgs/2021/03/03/x2c4oTEC.webp) 

多彩皮肤： ![](https://cdn.uzz5.com/imgs/2021/03/03/6z3Uy7lV.webp)

# 使用方法

程序启动后在窗口点击鼠标右键可以弹出右键菜单，主要功能都集中在这个菜单中。如果需要让它嵌入到任务栏显示，请勾选“显示任务栏窗口”。要显示CPU和内存利用率，请勾选“显示更多信息”。

# 自定义皮肤

![](https://cdn.uzz5.com/imgs/2021/03/03/rf3dT5zb.webp) 

在主窗口或通知区图标右键菜单上选择“其他功能”——“更换皮肤”可以打开更换皮肤界面. 

[点击此处](https://github.com/zhongyang219/TrafficMonitorSkin/blob/master/皮肤下载.md)可以下载更多皮肤。

用户还可以根据自己的需要编辑自己的皮肤。 皮肤文件放在程序所在目录的`skins`目录下，每个皮肤被放到单独的文件夹下，文件夹的名称就是皮肤的名称。 其中`background.bmp`和`background_l.bmp`是背景图片，`skin.ini`是皮肤的配置文件，可以通过`skin.ini`指定文本颜色、字体、皮肤作者、每个项目的大小和位置等信息。 

详细的皮肤制作教程请[点击此处](https://github.com/zhongyang219/TrafficMonitor/blob/master/皮肤制作教程.md)。 

推荐使用[皮肤编辑器](https://github.com/zhongyang219/TrafficMonitorSkinEditor/releases)来创建或编辑皮肤。

# 选项设置

![](https://cdn.uzz5.com/imgs/2021/03/03/A5hwn8lC.webp) 在右键菜单选择“选项...”可以进入选项设置。在选项设置对话框中，可以单独设置主窗口和任务栏窗口的文本颜色、字体、背景颜色、网速单位、显示的文本等。 

在“常规设置”选项卡中，可以设置是否在程序时自动检查更新，以及是否需要在开机是自动运行。可以设置在什么时候需要发出消息通知。 从1.72版本开始，支持每个项目文本颜色单独设置。勾选“指定每个项目的颜色”后，点击“文本颜色”右边的颜色框，会弹出详细颜色设置的对话框，可以在这里单独指定每个项目的颜色。