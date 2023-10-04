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

## Import - 数据导入

目前支持excel 文件导入, 后缀文件名 `.xlsx`，多Sheet管理, 其中`Guide`是创建根页指南, `Best`创建底层的 Best Guide指南.

Sheet 表名

- Guide
- Best 

[Import Demo: Guide.xlsx]({{site.url}}{{site.baseurl}}/assets/images/posts/best/guide.xlsx)

{: .warning }
> 注意`Guide`表格的`Create Best`列用于创建`Best Guide`主题父级页面，需要创建填`Yes`。 另外`Best`表格`Parent`如果填了关联，也会自动创建这个主题，不管Guide表格是否填了`Yes`值。

**导入提示:**

![Import Reports]({{site.url}}{{site.baseurl}}/assets/images/posts/index/guide-import.png)

**导入的数据:**
![Imported Data]({{site.url}}{{site.baseurl}}/assets/images/posts/best/import-data.jpg)


## Tab - 选项卡

### Content

{: .highlight }
> - Topic: 完整主题名，默认值为空，替代值在 `Sites -> Posts`[^1]中设置, H1标签中的内容。
- Subtitle: H1下显示的副标题
- Meta Title
- Meta Description
- Intro: 简介
- Filter by category description: 分类导航简介
- Conclusion: 总结


![Tab: Content]({{site.url}}{{site.baseurl}}/assets/images/posts/index/content.png)


#### Filter by category description
{: .fw-500 }

{: .highlight }
> 设置后可替代模版内容,如图中文字内容。


![Filter by categories]({{site.url}}{{site.baseurl}}/assets/images/posts/index/filter_by_categories.jpg)

#### Intro & Conclusion
{: .fw-500 }

{: .highlight }
> 设置后可替代模版内容

### Base Info

灰色状态表单为不可修改，父级guide创建时自动创建。

![Base Info]({{site.url}}{{site.baseurl}}/assets/images/posts/index/base_info.jpg)

{: .highlight }
> - List Type: 列表类型
- Name: 主题关键词
- Presentation: 相对主题的简写
- Featured: 精选
- Template: 重新指定模版
- Author: 作者（只能超级管理员修改）
- Children's Binding: 创建子页分组

#### List Type
{: .fw-500 }

{: .highlight }
> 用于`Schema`标记


#### Children's Binding
{: .fw-500 }

{: .highlight }
> 先在Binding[^2]中创建数据, 这里是对现有分组进行选择，而非直接创建。
Tab: Buying Guide, 创建此数据后才会出现的Tab
{: .fs-3 }

---

[^1]: [Best Guide Topic 默认值设置]({{site.url}}{{site.baseurl}}/docs/sites/post#topic).
[^2]: [Binding 子页分组管理]({{site.url}}{{site.baseurl}}/docs/binding).