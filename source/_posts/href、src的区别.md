---
title: href、src的区别
date: 2022-06-21
tags:
- HTML面试题
categories:
- 面试题
---


- href：  
表示超文本引用，指向网络资源，建立和当前元素或文档的链接关系。当浏览器识别到它指向的文件时，就会并行下载资源，不会停止对当前文档的处理。  
常在a、link标签中。


- src：  
表示资源引用，指向外部资源，指向的内容会嵌入到当前标签的位置。当浏览器解析到该元素时，会暂停其他资源的下载和处理，直到将该资源加载、编译、执行完毕，所以js脚本一般放在页面底部。