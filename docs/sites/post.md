---
layout: default
title: Post - 文章参数配置
nav_order: 3
parent: Sites - 站点配置
permalink: /docs/sites/post
---

# Post - 文章参数配置
{: .fs-9 .no_toc }

Topic, Meta Title / Description 默认值设置，支持`liquid`[^1]语法
{: .fs-6 .fw-300 }

---

## TABLE OF CONTENTS
{: .no_toc .text-delta }

1. TOC
{:toc}


![Sites -> posts]({{site.url}}{{site.baseurl}}/assets/images/sites/posts.png)

---

## Topic

主题设置范例

### Guide

```html
{%- raw -%}
A {{page.year}} Guide to {{page.name|pluralize}}
{% endraw -%}
```

### Best Guide

```html
{%- raw -%}
{% if page.depth == 1 %}Top {{page.number}} {{page.presentation}} {{page.year}}{% else %}{{page.name}} of {{page.year}}{% endif %}
{% endraw -%}
```

### Default Topic

```html
{%- raw -%}
{{page.name}}
{% endraw -%}
```

---

## Meta Title & Meta Description


---

[^1]: [Liquid 模版语法指南](https://shopify.github.io/liquid/basics/introduction/).