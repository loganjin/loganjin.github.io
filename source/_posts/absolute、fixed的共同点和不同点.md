---
title: absolute、fixed的共同点和不同点
date: 2022-06-28
tags:
- CSS面试题
categories:
- 面试题
---
（布局）


<!--more-->


- 共同点：  
    1. 改变行内元素的呈现方式，将display设置为inline-block。
    2. 使元素脱离普通文档流，不再占据文档物理空间。
    3. 覆盖非定位文档元素。


- 不同点：
    1. absolute和fixed的根元素不同，absolute的根元素可以设置，fixed的根元素是浏览器。
    2. 在有滚动条的页面中，absolute会跟着父元素进行移动，fixed固定在页面的具体位置。