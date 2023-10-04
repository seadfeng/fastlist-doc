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

### Sheet 表名

- Guide
- Best 

[Import Demo: Guide.xlsx]({{site.url}}{{site.baseurl}}/assets/images/posts/best/guide.xlsx)

{: .warning }
> - 注意`Guide`表格的**Create Best**列用于创建 (Best Guide) 主题父级页面，需要创建填`Yes`。 另外`Best`表格**Parent**如果填了关联，也会自动创建这个主题，不管Guide表格是否填了`Yes`值。
- **Taxon** 使用路径格式`Root Category / Child Category`，第一层分类必须人工在系统中创建，第一层之后会自动创建，需要谨慎填写（区分大小写，最好的办法是复制保持一致）。系统默认设定**最多两层**，超过两层分类页展示逻辑没有做处理。

### 导入后报告

报告中包含三项指标数据，注意里面是按分表报告，修正时不要看错了, `# 2` 是表中对应的行数**2**。

- Skip: 异常跳过，创建数据失败后的记录，正常情况会包含失败原因，方便做修正。
- Created: 实际创建
- Existed: 已存在，这里会包含重复数据（图中Sheet: Guide => #2, #3, #4 Slug值一样）

![Import Reports]({{site.url}}{{site.baseurl}}/assets/images/posts/index/guide-import.png)

### 导入的数据

{: .note }
> 这个例子中 "Best Proxy" 是被动创建的页面，表格不可以操控相关数据，需要修改数据在后台处理。

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

{: .note }
> 后台编辑创建步骤相对繁琐, 建议使用excel数据表来导入，效率会更高。

以下为人工编辑流程

1. 在Binding[^2]中预先创建数据
2. Binding分组进行选择(支持多选).
3. Children 中添加子级页面 (子页数量超过600不能用这个操, TODO: 后续解决，数量多通过数据表添加最佳)
4. 子级页面添加选择`Binding`，这里有两个地方可以进行编辑:
  - Tab: Children - 当前页 ![ Tab: Children]({{site.url}}{{site.baseurl}}/assets/images/posts/best/children-tab.jpg)
  - Child edit page => Tab: Bindings - 进入子级页面编辑 ![ Child => Tab: Bindings]({{site.url}}{{site.baseurl}}/assets/images/posts/best/child-binding-tab.jpg)


#### Buying Guide
{: .fw-500 }

[Children's Binding](#childrens-binding) 数据创建后才会出现这个选项卡
{: .fs-3 }


数据排序在右侧边栏，有两项排序可以拖拽操作。

![Binding Sorting]({{site.url}}{{site.baseurl}}/assets/images/posts/best/binding-sorting.jpg)

---

[^1]: [Best Guide Topic 默认值设置]({{site.url}}{{site.baseurl}}/docs/sites/post#topic).
[^2]: [Binding 子页分组管理]({{site.url}}{{site.baseurl}}/docs/binding).