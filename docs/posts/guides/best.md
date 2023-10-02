---
layout: default
title: Best Guide
nav_order: 2
parent: Posts - 文章
permalink: /docs/posts/guides/best
---

# Best Guide - 最佳指南
{: .fs-9 .no_toc }

包含了Top list模块，子页也一样包含。
{: .fs-6 .fw-300 }

---

## TABLE OF CONTENTS
{: .no_toc .text-delta }

1. TOC
{:toc}

---


## Tab - 选项卡

### Content

- Topic: 完整主题名，默认值为空，替代值在 `Sites -> Posts`[^1]中设置, H1标签中的内容。
- Subtitle: H1下显示的副标题
- Meta Title
- Meta Description
- Intro: 简介
- Filter by category description: 分类导航简介
- Conclusion: 总结


![Tab: Content]({{site.url}}{{site.baseurl}}/assets/images/posts/index/content.png)


#### Filter by category description
{: .fw-500 }

设置后可替代模版内容,如图中文字内容。
{: .fs-3 }

![Filter by categories]({{site.url}}{{site.baseurl}}/assets/images/posts/index/filter_by_categories.jpg)

#### Intro
{: .fw-500 }

设置后可替代模版内容
{: .fs-3 }

#### Conclusion
{: .fw-500 }

设置后可替代模版内容
{: .fs-3 }

### Base Info

灰色状态表单为不可修改，父级guide创建时自动创建。

- List Type: 列表类型
- Name: 主题关键词
- Presentation: 相对主题的简写
- Featured: 精选
- Template: 重新指定模版
- Author: 作者（只能超级管理员修改）
- Children's Binding: 创建子页分组

![Base Info]({{site.url}}{{site.baseurl}}/assets/images/posts/index/base_info.jpg)

#### List Type
{: .fw-500 }

用于`Schema`标记
{: .fs-3 }

#### Children's Binding
{: .fw-500 }

Binding 中先创建数据，这里是对现有分组进行选择，而非直接创建。

Tab: Buying Guide, 这是在Best Guide下创建才出现的 Tab, 其他类型如果创建暂时未处理
{: .fs-3 }

---

[^1]: [Best Guide Topic 默认值设置]({{site.url}}{{site.baseurl}}/docs/sites/post#topic).