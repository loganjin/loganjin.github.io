---
title: Hexo博客框架Front-matter语法
date: 2022-06-18
tags:
- Hexo
categories:
- 程序员的自我修养
---


Front-matter is a block of Markdown at the beginning of the file that is used to configure settings for your writings. Front-matter is terminated by three dashes:
```
---
title: Hello World
date: 2013/7/13 20:46:25
categories:
- programmer
tags:
- Hexo
---
```


<!--more-->


## Setting
> title
> date: published date   
> categories  
> tags  


## 常见问题  
- 使类别并列产生：  
```
categories:
- [programmer]
- [Front-End]
```
