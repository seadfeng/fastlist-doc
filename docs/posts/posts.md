---
layout: default
title: Posts - 文章
nav_order: 3
has_children: true
permalink: /docs/posts
---

# Posts - 文章
{: .fs-9 }

文章层级最大深度为两层，顶层深度为0. 目前顶层文章类型只有**guide**
{: .fs-6 .fw-300 }

## 常见通用字段

### Intro - 文章简介

文章简介，所有类型几乎一样，best 类型比较特殊，留空时会使用文字模版。


### Filter by category description - 二级子页分组内容介绍

子页分组后导航模块内容,常用于Best guide 父级页面.

![Filter by categories](/assets/images/posts/index/filter_by_categories.jpg)

### Sections - 章节 H2 段落

- Section Heading: 章节标题
- Toc name: 目录名
- Body: 段落内容

### Conclusion - 文章结尾

Best 类型一般设定了文字自动模版，此字段用于替换文字模版内容。 其他类型文章直接用Sections添加 Conclusion章节


