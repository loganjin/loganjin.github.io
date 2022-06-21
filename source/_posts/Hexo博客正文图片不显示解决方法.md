---
title: Hexo博客正文图片不显示解决方法
date: 2022/6/21
tags:
- Hexo
categories:
- 程序员的自我修养
---


将图片放在`source/images`文件夹中，通过类似于`![](/images/image.jpg)`的Markdown语法来访问它们，发现图片在博客正文不显示。  
注：  
Hexo version: 5.4.2  
NexT version: 8.12.1


<!--more-->


解决方法：  
将_config.yml中的`post_asset_folder`设置为true，通过命令行新建文章，将图片放在伴随命令行指令产生的文件夹中，在通过如`{% asset_img example.jpg This is an example image %}`的标签插件来引入图片即可。


