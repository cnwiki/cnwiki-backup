---
title: 编辑指南
description: 
published: true
date: 2020-04-28T01:19:33.703Z
tags: 
---

欢迎加入赤纳维基！任何人都可以编辑赤维的页面，而该指南可以帮你更好地做到这一点。
# 编辑器
赤维使用的wiki.js系统当前支持三种编辑器，他们分别是：markdown、html、visual editor。

## markdown
markdown编辑器足以胜任大部分页面的撰写工作。其功能远少于mediawiki的wikitext，不过因此语法也简单很多。
markdown的学习资料有:
- https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf （注：本站无法使用该文档内的emoji功能）
- https://www.markdownguide.org
- https://www.jianshu.com/p/q81RER （墙内链接，请手动复制到新的窗口）

## html
若你所编辑的页面需要用到更复杂的排版的话（例如[词典](/zh/dictionary)页面所用到的三纵列布局），你应该选择该编辑器。
目前，每个页面都被注入了下列css class来方便排版。[首页](/zh/home)使用了前两个class，而[爱国数据库](/zh/nationalismdb)则使用了后两个类。你可以前往这些页面，点击右上角操作->源文件来查看使用实例。
```css
.c-grid {
  display: grid
}
.home-grid {
  grid-template-columns: repeat(auto-fit,minmax(300px,1fr));
  grid-gap: 10px
}
.c-flex {
  display: flex;
  flex-wrap: wrap
}
.home-flex > div {
  width: 400px;
  flex-grow: 1
}
```


## visual editor
理论上所有该编辑器能做到的效果markdown+少许css也能做到。我们强烈建议用户先尝试学习和使用markdown。不过若你依然觉得visual editor是用起来最方便的话我们也不会阻止你用。
# 多语言及页面url路径
秉承着“讲好中国故事，传播好中国声音”的精神，赤纳维基一直把将中国民族主义崛起的故事推广给国际友人的目标置于首位。因此，本站同时支持简体中文和英文，并可能在未来加入对更多语言的支持。
## 语言代码
系统根据每个页面的url（中文名为[统一资源定位符](https://zh.wikipedia.org/wiki/统一资源定位符)）来判定其内容的语言。假设其url的路径以/zh打头，那么页面语言就为简体中文。反之，若路径的开头是/en则说明页面内容为英文。