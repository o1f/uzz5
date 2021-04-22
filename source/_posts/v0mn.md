---
title: 'MyDockFinder : 体验极致模拟Mac OS系统桌面'
date: 2021-1-19 20:02:33
categories:
  - - Win
tags:
  - 工具
  - 系统
id: '34'
thumbnail: https://cdn.uzz5.com/imgs/2021/02/28/ohtDtDNn.webp
abbrlink: v0mn
---


这是一款真正意义上的把Windows变成MacOS的软件，不用更换主题，不用修改Dll，直接是程序接管了Explorer，比任何美化主题都简单，高效。主要是为Win10开发的软件，但是也兼容低版本系统，如Win7。软件还提供全套的Mac OS图标，要完全给Windows换皮也是可以的！ 软件包括Dock（底下部分）和Finder（顶上部分），其中Dock的功能已经全部完成，Finder还在写，但是已经能实现比如蓝牙，WIFI，亮度，声音等功能了，而且也能接管程序的操作菜单栏（左上角）。主流社交软件的消息提醒也支持，具体的请见官网。如果嫌弃Finder未完成，也可以在设置里面关闭，只用Dock。 软件的本质是在桌面上加了两个组件，所以不会对原本的系统做任何改变。第一次进入软件可能会发现Dock特别小，在Dock的空白处单击右键进入设置，里面把图标大小调整成100就好了。还有其他的动画、效果之类的设置也在里面，根据自己电脑的配置调整就好了。 关于软件的开发进度： Dock已经是没问题了，Finder目前在更新右上角的功能，左上角的还是Bug一堆，估计还要等几个月。

# 官网

[https://www.mydockfinder.com/](https://www.mydockfinder.com/) 

[下载地址](https://www.mydockfinder.com/index.php/%E4%B8%8B%E8%BD%BD%E4%B8%AD%E5%BF%83/)

# 介绍及预览

## 系统级模糊效果

完美支持最新版Win10 20H2系统，可使用系统级模糊效果，Win10 1803以上系统可使用高斯模糊，Win7系统和老版本Win10为Aero毛玻璃效果。 ![](https://cdn.uzz5.com/imgs/2021/02/28/hd2vMAwE.webp)

## 运行程序图标显示窗口预览

所有运行图标并且有窗口的程序可以鼠标悬停后显示窗口预览（支持Win10UWP程序）需要在Dock偏好设置-预览中开启，可自定义预览大小及延迟时间。 ![](https://cdn.uzz5.com/imgs/2021/02/28/Lq6Ex81C.webp)

## 文件(夹)直接拖放进Dock

所有文件(包括UWP快捷方式)及文件夹可直接托放进Dock中，可多个文件(夹)批量拖入；管理员账号Administrator和管理员模式运行时不会有此动画效果，所以不建议使用管理员账号和管理员模式运行。 ![](https://cdn.uzz5.com/imgs/2021/02/28/Ws4eTfZq.webp)

## 微信、QQ、钉钉消息提示

支持QQ、TIM、微信（UWP微信）、阿里旺旺、YY等软件消息计数和提示效果，此消息计数算法为原创QQ等其他软件并没有公开接口所以不能显示具体聊天内容。 ![](https://cdn.uzz5.com/imgs/2021/02/28/oG2kAmhk.webp)

## 显示当前城市天气

添加系统图标-实时天气 可添加天气图标，使用高德地图API自动定位并获取实时及未来天气，Dock图标为实时天气 预览窗口为未来天气，所以图标会和预览显示天气有所出入。 ![](https://cdn.uzz5.com/imgs/2021/02/28/KfBQ5P8w.webp)

## 图标显示任务进度

支持复制文件、Chrome等浏览器下载、Foobar播放音乐、Potplayer播放视频等，当系统任务栏窗口图标显示进度时，Dock中对应的图标就会显示进度条。 Dockmod必须运行 ![](https://cdn.uzz5.com/imgs/2021/02/28/kVLqQE2b.webp)

### 窗口最小化到DOCK

自带三种窗口最小化效果99%模拟Mac窗口动画，可在Dock偏好设置-最小化中勾选开启，最小化动画采用D3D硬件加速渲染，Win8以上系统可以使用完整DX11效果。 Dockmod必须运行 ![](https://cdn.uzz5.com/imgs/2021/02/28/UZL23GWD.webp) ![](https://cdn.uzz5.com/imgs/2021/02/28/8FG31uzk.webp) ![](https://cdn.uzz5.com/imgs/2021/02/28/u1Aw3CPI.webp)

## 显示完整文件夹内容

添加文件夹后图标右键菜单可修改显示文件夹内缩略图和文件内容排序方式，左键点击可显示完成文件夹内所有文件，点击文件夹内二级目录可再次显示下级目录所有文件，文件名显示不全时鼠标悬停后可显示全部名称；支持绝大多数视频格式（需要下载Opencv\_ffmpeg410.Dll视频解码文件），文件夹中的文件还支持拖拽操作可以直接鼠标拖出移动或复制。 ![](https://cdn.uzz5.com/imgs/2021/02/28/N0VQmxjK.webp) ![](https://cdn.uzz5.com/imgs/2021/02/28/eZbePPu4.webp)