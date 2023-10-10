---
layout: default
title: Api
nav_order: 8
has_children: false
permalink: /docs/api
---

# Api
{: .fs-9 }

支持火车头采集发布

{: .warning }
> 图片上传暂不支持

## 创建Token

1. 菜单`Settings => Api Tokens`
2. New Api Token


## 火车头发布接口

全局变量填token值, 登陆方式免登陆

### Fastlist-V1-Taxon

获取分类列表返回的是Taxon分类

![Taxon分类发布接口]({{site.url}}{{site.baseurl}}/assets/images/api/1ad938bb70a0f9c35916285dbd090cf9.png)


### Fastlist-V1

获取分类列表返回的是 `Guide` 文章类型