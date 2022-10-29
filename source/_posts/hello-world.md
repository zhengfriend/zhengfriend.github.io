---

title: 博客还在魔改中啊啊啊
date: 2022-10-27 16:17:41
cover: /img/heike/heike1.jpg
---
{% note no-icon %}
博客还在主题魔改中......
{% endnote %}

博客初步搭好了，祖传的Hello World必须要来一下吧。

## Front-matter

Front-matter 是 markdown 文件最上方用三个短横线(---)分隔的区域，用于指定个别文档的变数。
- Page Front-matter 用于页面配置
- Post Front-matter 用于文章配置

###  Page Front-matter 页面配置

```markdown 

---
title:
date:
updated:
type:
comments:
description:
keywords:
top_img:
mathjax:
katex:
aside:
aplayer：
highlight_shrink：
---

```

|写法|解释|
|:---|:---|
|title|【必须】页面标题|
|date|【必须】页面创建日期|
|type|【必须】标签、分类和友情链接三个页面需要配置|
|updated|【可选】页面更新日期|
|description|【可选】页面描述|
|keywords|【可选】页面关键字|
|comments|【可选】显示页面评论模块(默认 true)|
|top_img|【可选】页面顶部图片|
|mathjax|【可选】显示mathjax(当设置mathjax的per_page: false时，才需要配置，默认 false)|
|katex|【可选】显示katex(当设置katex的per_page: false时，才需要配置，默认 false)|
|aside|【可选】显示侧边栏 (默认 true)|
|aplayer|【可选】在需要的页面加载aplayer的js和css,请参考文章下面的音乐 配置|
|highlight_shrink|【可选】配置代码框是否展开(true/false)(默认为设置中highlight_shrink的配置)|


###  Post Front-matter 文章配置

```markdown

---
title:
date:
updated:
tags:
categories:
keywords:
description:
top_img:
comments:
cover:
toc:
toc_number:
toc_style_simple:
copyright:
copyright_author:
copyright_author_href:
copyright_url:
copyright_info:
mathjax:
katex:
aplayer:
highlight_shrink:
aside:
---

```

|写法|解释|
|:---|:---|
|title|【必须】文章标题|
|date|【必须】文章创建日期|
|updated|【可选】文章更新日期|
|tags|【可选】文章标签|
|categories|【可选】文章分类|
|description|【可选】文章描述|
|keywords|【可选】文章关键字|
|top_img|【可选】文章顶部图片|
|cover|【可选】文章缩略图(如果没有设置top_img,文章页顶部将显示缩略图，可设为false/图片地址/留空)|
|comments|【可选】是否显示文章评论模块(默认 true)|
|toc|【可选】是否显示文章TOC(默认为设置中toc的enable配置)|
|toc_number|【可选】显示toc_number(默认为设置中toc的number配置)|
|toc_style_simple|【可选】显示 toc 简洁模式|
|copyright|【可选】显示文章版权模块(默认为设置中post_copyright的enable配置)|
|copyright_author_href|【可选】文章版权模块的文章作者链接|
|copyright_url|【可选】文章版权模块的文章连结链接|
|copyright_info|【可选】文章版权模块的版权声明文字|
|mathjax|【可选】显示mathjax(当设置mathjax的per_page: false时，才需要配置，默认 false)|
|katex|【可选】显示katex(当设置katex的per_page: false时，才需要配置，默认 false)|
|aside|【可选】显示侧边栏 (默认 true)|
|aplayer|【可选】在需要的页面加载aplayer的js和css,请参考文章下面的音乐 配置|
|highlight_shrink|【可选】配置代码框是否展开(true/false)(默认为设置中highlight_shrink的配置)|

## 标签页
1. 进入Hexo博客根目录，打开cmd命令窗口，执行命令：hexo new page tags
2. 在目录【Hexo博客根目录/source/】下，自动创建 一个包含 index.md 文件 的 tags 目录
3.  未完待续。。。。。。
