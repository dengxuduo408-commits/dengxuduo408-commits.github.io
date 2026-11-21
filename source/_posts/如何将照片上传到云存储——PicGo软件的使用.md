---
title: 如何将照片上传到云存储——PicGo软件的使用
tags:
  - PicGo
  - 照片
categories:
  - 软件使用
thumbnail: "https://cdn.jsdelivr.net/gh/dengxuduo408-commits/image-bed@main/img/20261122010119490.jpg"
date: 2026-11-22 00:58:59
---
# 基本概念介绍
- 图床：专门用来*存放图片的网上网盘*，并且给你生成一个**公开网址（直链）**，别人（浏览器）通过这个网址就能直接打开图片。
其底层存储大多选择GitHub仓库

- CDN：一批分布在全国、全球各地的缓存服务器，作用是**加速加载图片**。e.g. jsDelivr就是一个免费的CDN,专门加速 GitHub 上的静态资源（图片、js、css）。

- link分类：
1、图片直链（即URL）：图片本身的真实地址，浏览器访问这个地址，直接加载图片二进制，页面上就显示一个图片；所有人都能访问。
https://cdn.jsdelivr.net/gh/dengxuduo408-commits/image-bed@main/img/20261121173036439.png
2、各种语法包装的代码（包裹了地址）：
  - markdown链接：![描述]（直链）
  - HTML语法：<img src="直链">
3、公网直链vs本地路径
公网直链：https://cdn.jsdelivr.net/gh/xxx/image-bed@main/img/test.png 本质是**互联网上一台公开服务器**上的文件。任何人只要能上网，都能访问这个图片。
本地路径：C:\blog\photo\test.jpg 本质是**电脑硬盘**里的文件，只在这台电脑上看得见，别人访问不了。

# PicGo软件
所以如何让别人访问到自己电脑里的本地文件呢，就要转本地路径为公网直链，即把文件上传到**云存储**：各网盘、github等。在此我用的时PicGo软件，让它帮我上传到github中专门储存照片的repo里。
整套流程：用PicGo软件把电脑本地的一张照片上传到你的GitHub里专门放图床的仓库，PicGo再生成各种格式的CDN链接，就可以粘贴进Markdown文章里。



