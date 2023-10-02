---
layout: default
title: Base - 站点基础配置
nav_order: 1
parent: Sites - 站点配置
permalink: /docs/sites/base
---

# Base - 站点基础配置
{: .fs-9 .no_toc }

Meta 信息为缺省时使用，一般情况用不上，具体页面Meta在模版管理中设置
{: .fs-6 .fw-300 }

## 目录
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Site Name -  站点全称

{%- raw -%}
*Demo Site*, 编辑器中使用变量: {{site.name}}
{% endraw -%}

```html
{%- raw -%}
Design By {{site.name}}
# Ouput: Design By Demo Site
{% endraw -%}
```

## Site Alias -  站点别名

{%- raw -%}
*DemoSite*, 编辑器中使用变量: {{site.alias}}
{% endraw -%}

```html
{%- raw -%}
Design By {{site.alias}}
# Ouput: Design By DemoSite
{% endraw -%}
```

## Site Name Abbreviation - 站点大写字母缩写

{%- raw -%}
*DS*, 编辑器中使用变量: {{site.abbreviation}}
{% endraw -%}

```html
{%- raw -%}
{{site.abbreviation}} Score
# Ouput: DS Score
{% endraw -%}
```

## Meta title

title 缺省时使用

```html
<title>Meta title</title>
```
## Meta description

meta description 缺省时使用

```html
<meta name="description" content="Meta description">
```

