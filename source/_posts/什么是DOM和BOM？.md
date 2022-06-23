---
title: 什么是DOM和BOM？
date: 2022-06-23
tags:
- JS面试题
categories:
- 面试题
---
（Web APIs）


<!--more-->


- DOM：  
指的是文档对象模型，它指的是把文档当做一个对象，这个对象主要定义了处理网页内容的方法和接口。


- BOM：  
指的是浏览器对象模型，它指的是把浏览器当做一个对象来对待，这个对象主要定义了与浏览器进行交互的方法和接口。    
BOM的核心是window，而window对象具有双重角色，它既是js访问浏览器窗口的一个接口，又是一个全局（Global）对象，定义在全局作用域中的变量、函数都会变成window对象的属性和方法。window对象含有location对象、navigator对象、screen对象等子对象，并且DOM的最根本的对象document对象也是window对象的子对象。
