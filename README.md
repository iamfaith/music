# 音乐搜索器

[![GitHub release](https://img.shields.io/github/release/maicong/music.svg?style=flat-square)](https://github.com/maicong/music/releases)
[![PHP version](https://img.shields.io/badge/php-%3E%205.4-orange.svg)](https://github.com/php-src/php)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](#LICENSE)

> **⚠️ 项目开源，请勿商用**

## 说明

麦葱特制多站合一音乐搜索解决方案，支持搜索试听以下网站音乐：

[网易云音乐](http://music.163.com) [QQ音乐](http://y.qq.com) [酷狗音乐](http://www.kugou.com) [酷我音乐](http://www.kuwo.cn) [虾米音乐](http://www.xiami.com) [百度音乐](http://music.baidu.com) [一听音乐](http://www.1ting.com) [咪咕音乐](http://music.migu.cn) [荔枝FM](http://www.lizhi.fm) [蜻蜓FM](http://www.qingting.fm) [喜马拉雅FM](http://www.ximalaya.com) [全民K歌](http://kg.qq.com) [5sing原创](http://5sing.kugou.com/yc) [5sing翻唱](http://5sing.kugou.com/fc)

数据调用的是各网站的 API 接口，有的接口并不是开放的，随时可能失效，本项目相关代码仅供参考。

## 演示

[http://music.2333.me/](http://music.2333.me/ "音乐搜索器")

如果获取有误或需要改进，欢迎提交 [Issues](https://github.com/maicong/music/issues)

## 下载

[📦 下载开发版](https://github.com/maicong/music/archive/master.zip) [📦 获取稳定版](https://github.com/maicong/music/releases)

## 解决方案

**1. 提示数据获取失败**

方案1：

```
修改 index.php 文件里的 MC_PROXY 为您的代理地址
将 core/music.php 里需要代理的 URL 'proxy' => false 改为 'proxy' => true
```

方案2：

```
在 core/music.php 里查找 setTimeout，将其后面的数值 20 改为更大。
在 static/js/music.js 里查找 `timeout`，将其数值 30000 改为更大。
```

方案3：

```
服务器要支持 curl。
更换服务器，选择延迟更低的服务器。
```

## 更新日志

请查看 [CHANGELOG.md](CHANGELOG.md)

## 免责声明

1. 本站音频文件来自各网站接口，本站不会修改任何音频文件
2. 音频版权来自各网站，本站只提供数据查询服务，不提供任何音频存储和贩卖服务

## 开源协议

The MIT License (MIT)
