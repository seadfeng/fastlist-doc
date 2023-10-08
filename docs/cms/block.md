---
layout: default
title: Block - 块
nav_order: 2
parent: CMS - 内容管理
permalink: /docs/cms/block
---

# Block - 块
{: .fs-9 .no_toc }

用于页面通用模块，比如常见的Footer模块。
{: .fs-6 .fw-300 }

{: .warning }
> - 权限设置注意控制，不要分配给内容编辑，以免错误操作
- 编辑重要内容时要**做好源码备份**，一旦出错便于还原。

---

## TABLE OF CONTENTS
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## 菜单/路径

Menu: Cms / Block 


## Layout - 系统布局

Identity: `layout_*`， layout_ 开头不允许删除

### Header

页顶 & 导航

Block Identity: `layout_header`

{: .note }
> LOGO宽度设置，根据站点logo长度调整（不是填实际图片长度，而是手工调整大小来适应导航条）


```html
{%- raw -%}
{% render "silicon/header/navbar" site: site, logo_width: 40, nav_dark: false %}
{% endraw -%}
```

### Footer

页底

Identity: `layout_footer`

