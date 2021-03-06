---
title: Hexo博客框架NexT主题美化
date: 2022-06-18
tags:
- Hexo
categories:
- 程序员的自我修养
---


## _config.yml
After the installation of Hexo and NexT, you may found that there are two configuration files using by Hexo and both called `_config.yml`: The first one is under site root directory, which contains Hexo's config. The second one is under theme root directory, which is provided by NexT and contains theme's config. Let's call the first one – `Hexo config file`, and the second one – `NexT config file`.  

We do not recommend directly modifying the `NexT config file`. It is quite often running into conflict status when updating NexT theme via git pull, or need to merge configurations manually when upgrading to new releases. For the theme installed through npm, it is also difficult to modify the NexT config file in node_modules.  

In order to resolve this issue, we recommend using the [Alternate Theme Config](https://hexo.io/docs/configuration.html#Alternate-Theme-Config) feature to configure theme NexT.

We strongly recommend you to store your theme configuration in one place. But in case you have to store your theme configuration separately, you need to know the priority of those configurations: The theme_config inside site’s primary configuration file has the highest priority during merging, then the dedicated theme configuration file.
The _config.yml file under the theme directory has the lowest priority.


<!--more-->


## _config.yml美化
> title: LIFE×WORK  
> subtitle: '知命不惧，日日自新'  
> description: '嘿，开心一点嘛'  
> author: Logan Jin  
> language: en  
> timezone: 'Asia/Shanghai'  
> highlight->auto_detect 
> theme: next  


## _config.next.yml美化
> scheme: Gemini  
> darkmode: true  
> favicon: 建军  
> menu: home、categories、tags     
> menu_settings: badges  
> avatar: me  
> social: Github、E-Mail、Bilibili、Instagram     
> footer: 
> 
> > since  
> > icon->animated  
> 
> back2top: scrollpercent  
> canvas_ribbon
> npm install hexo-generator-searchdb  
> hexo new page tags  
> tag_icon: true  
> 帖子部分显示，存在显示全文：<!--more-->



