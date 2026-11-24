---
title: Markdown画流程图——Mermaid语法
tags:
  - Markdown
  - Mermaid
  - 画图
categories:
  - Markdown
thumbnail: "https://cdn.jsdelivr.net/gh/dengxuduo408-commits/image-bed@main/img/20261124225729168.png"
date: 2026-11-23 13:26:57
---
想在文章中画流程图、关系图，使用以下markdown语法即可：
![](https://cdn.jsdelivr.net/gh/dengxuduo408-commits/image-bed@main/img/20261125002739773.png)

```mermaid
  graph TD
    A-->B
    A-->C
    B-->D
    C-->D
```
更多语法可以参考 Mermaid JS 官网：https://mermaid.js.org/ 。