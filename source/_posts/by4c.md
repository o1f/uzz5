---
title: 文章名
date: 时间
categories:
  - - Web
tags:
  - bilibili
  - 插件
  - 油猴
id: '74'
thumbnail:
---


开源地址： [https://github.com/the1812/Bilibili-Evolved](https://github.com/the1812/Bilibili-Evolved) 建议反馈： [https://github.com/the1812/Bilibili-Evolved/issues](https://github.com/the1812/Bilibili-Evolved/issues) 强大的哔哩哔哩增强脚本: 下载视频, 音乐, 封面, 弹幕 / 简化直播间, 评论区, 首页 / 自定义顶栏, 删除广告, 夜间模式 / 触屏设备支持

# 安装

需要浏览器拥有 [Tampermonkey](https://tampermonkey.net/) 插件. 点击名称即可安装

[正式版](https://cdn.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/bilibili-evolved.user.js)

[预览版](https://cdn.jsdelivr.net/gh/the1812/Bilibili-Evolved@preview/bilibili-evolved.preview.user.js)

[离线版](https://cdn.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/bilibili-evolved.offline.user.js)

[预览离线版](https://cdn.jsdelivr.net/gh/the1812/Bilibili-Evolved@preview/bilibili-evolved.preview-offline.user.js)

正式发布的版本, 最稳定, 更新频率较低.

新增内容测试的地方, 更新频率高, 但功能不稳定.

内置所有依赖项, 体积较大, 更新频率高于正式版.

兼备预览版和离线版的特点.

> 使用过程中脚本管理器可能会提示"脚本试图访问跨域资源", 请选择"始终允许". 某些破坏性的大更新会使旧版脚本**完全**无法运行, 请及时检查更新. 自 2021 年 (v1.11.12) 起, 脚本不再在 GreasyFork 开放入口, 所有的后续更新均以 GitHub 上的信息为准.

## 备用安装源

如果默认的安装链接无法使用, 可以尝试以下的备用安装源.

更新延迟

下载速度

正式版

预览版

离线版

预览离线版

jsDelivr

24h

快

[安装](https://cdn.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/bilibili-evolved.user.js)

[安装](https://cdn.jsdelivr.net/gh/the1812/Bilibili-Evolved@preview/bilibili-evolved.preview.user.js)

[安装](https://cdn.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/bilibili-evolved.offline.user.js)

[安装](https://cdn.jsdelivr.net/gh/the1812/Bilibili-Evolved@preview/bilibili-evolved.preview-offline.user.js)

GitHub

<1h

需要梯子

[安装](https://github.com/the1812/Bilibili-Evolved/raw/master/bilibili-evolved.user.js)

[安装](https://github.com/the1812/Bilibili-Evolved/raw/preview/bilibili-evolved.preview.user.js)

[安装](https://github.com/the1812/Bilibili-Evolved/raw/master/bilibili-evolved.offline.user.js)

[安装](https://github.com/the1812/Bilibili-Evolved/raw/preview/bilibili-evolved.preview-offline.user.js)

## 推荐配置

*   操作系统: 64-bit Windows 10 / macOS 10.15+
*   分辨率: 2K+ / 192ppi
*   浏览器: Chrome 80+ / Firefox 65+ / Edge 80+ / Safari 14+
*   处理器: Intel Core i7 / AMD Ryzen 5
*   内存: 8GB
*   脚本管理器: Tampermonkey 4.11 / Violentmonkey 2.12
*   显卡: GeForce GTX 660 / Radeon HD 7870
*   网络: 10MB/s

# 设置

脚本启用后, 在网页左侧中央会有一个齿轮图标, 点击即可打开设置. 默认只启用了一部分功能, 您可以根据需要自由调整设置. 可以在[功能列表](doc/features.md)页中查看每项功能的详细说明, 在网页中通过鼠标停留在某一项也可以查看简要说明. 大部分功能可通过设置面板开启, 有一些功能会以`附加功能`的形式生效, 或者是可以在`附加功能`做进一步设置. `附加功能`可从网页左侧中央的功能按钮进入. **绝大部分设置保存后, 需要刷新网页才能生效. 仅有一些样式设置可以立即生效.** ![请输入图片描述](https://cdn.uzz5.com/imgs/2021/02/28/5bPBkCbO.webp "请输入图片描述")

# 兼容性

## 脚本管理器

### [Tampermonkey](https://tampermonkey.net/) / [Violentmonkey](https://violentmonkey.github.io/)

完全兼容, 但在较旧的浏览器中 Violentmonkey 可能无法运行此脚本.

### [Greasemonkey](https://www.greasespot.net/)

可以安装, 但是由于 Greasemonkey 4 只允许脚本在页面完全加载后运行, 样式相关功能体验会比较糟糕, 比如打开夜间模式后每个页面在完全加载之前都是亮色的. 所以还是强烈建议您使用上述的两种脚本管理器.

### [AdGuard](https://adguard.com/zh_cn/adguard-windows/overview.html)

不兼容.

## 浏览器

支持**最新版** Chrome, Edge (Chromium 内核), Firefox, Safari, 不保证脚本能在["套壳类浏览器"](https://www.jianshu.com/p/67d790a8f221)或者较长时间没更新的浏览器中完美运行. UWP 版 Edge 已经不再支持了(就是 Windows 10 自带的那个), 请使用以上列出的浏览器, 或换用 [Chromium 内核的 Edge](https://www.microsoft.com/en-us/edge).

> Windows 10 20H2 更新中好像完全替换掉了 UWP 版 Edge (R.I.P.) 自带浏览器变成了 Chromium 内核 Edge.

# 已知问题

*   和`解除B站区域限制`一同使用时, 两个脚本功能互相没有任何问题, 但有的人会遇到没弹幕的状况. 单独使用各脚本时正常, 目前未找到原因.
*   4K视频只能导出下载, 不能直接下载.
*   可能无法很好地适应窄屏幕, 请尽量以1400px以上的宽度使用此脚本.
*   ASS弹幕下载不能包含高级弹幕, 字幕弹幕等.

# 相关推荐

这些脚本/插件同样能够改善您在B站的体验, 相同的功能将不会整合到 Bilibili Evolved, 但会尽可能地适配

## bilibili网页端添加APP首页推荐

作者: [indefined](https://github.com/indefined)

*   [GitHub](https://github.com/indefined/UserScripts/tree/master/bilibiliHome)
*   [GreasyFork](https://greasyfork.org/zh-CN/scripts/368446-bilibili%E7%BD%91%E9%A1%B5%E7%AB%AF%E6%B7%BB%E5%8A%A0app%E9%A6%96%E9%A1%B5%E6%8E%A8%E8%8D%90)

## pakku.js 哔哩哔哩弹幕过滤器

作者: [xmcp](https://github.com/xmcp)

*   [主页](https://s.xmcp.ml/pakkujs/)
*   [GitHub](https://github.com/xmcp/pakku.js)

## BLTH - Bilibili Live Tasks Helper

作者: [andywang425](https://github.com/andywang425)

*   [GitHub](https://github.com/andywang425/BLTH)
*   [GreasyFork](https://greasyfork.org/zh-CN/scripts/406048-b%E7%AB%99%E7%9B%B4%E6%92%AD%E9%97%B4%E6%8C%82%E6%9C%BA%E5%8A%A9%E6%89%8B)

* * *

**喜欢的话就点个Star吧(°∀°)ﾉ** 本文仅做分享，更多请访问开源项目地址~