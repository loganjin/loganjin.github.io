---
title: 对比methods和computed
date: 2022/6/23
tags:
- Vue面试题
categories:
- 面试题
---
（基础知识）


<!--more-->


- 相同点：  
methods和computed最终结果相同。


- 不同点：  
computed会进行`缓存`,多次使用会观察有没有变化：没有变化就直接返回原有结果，不会重新调用，有变化会重新调用一次；methods每次使用都会调用一次。

