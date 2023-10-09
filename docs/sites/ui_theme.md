---
layout: default
title: UI & Theme
nav_order: 1
parent: Sites - 站点配置
permalink: /docs/sites/theme
---

# UI & Theme - 模版配置
{: .fs-9 }

LOGO可使用svg图标

{: .warning }
> 上传logo后，需要修改导航条LOGO的宽度([Block Header])，如底部模块也使用了此logo一并修改。

- Favicon PNG: 站点图标，宽高比例1:1，最小值 (310x310px)
  - {{site.icon}}
- Logo: 可使用svg图标 
  - {{site.logo}}
- Reverse Logo: 反色LOGO，用于深色背景，UI设计套装正常情况是必须包含的。 
  - {{site.reverse_logo}}
- Tile Color: Windows 保存站点到桌面时，会使用Favicon PNG图标，这个颜色是图标的底色（时间太久了不一定对=，= ）。
- Theme: 主题模版

---

图变量形式
```ruby
{%- raw -%}
{ 
  'medium' => {'url' => '', 'content_type' => '', 'height' => '', 'width' => ''} ,
  'thumbnail' => {'url' => '', 'content_type' => '', 'height' => , 'width' => ''} 
}
{% endraw -%}
```

liquid demo:
```liquid
{%- raw -%}
<img src="{{site.icon.medium.url}}" width="{{site.icon.medium.width}}" height="{{site.icon.medium.height}}" />
{% endraw -%}
```
---
[Block Header]: {{site.url}}{{site.baseurl}}/docs/cms/block#header