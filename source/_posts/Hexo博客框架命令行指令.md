---
title: Hexo博客框架命令行指令
date: 2022-06-21
tags:
- Hexo
categories:
- 程序员的自我修养
---


- 创建新文章
```
$ hexo new [layout] <title>
```
拓：  
|  布局（layout）   | 路径  |
|  ----  | ----  |
| post  | source/_posts |
| page  | source |
| draft  | source/_drafts |


<!--more-->


- 清除缓存文件 (db.json) 和已生成的静态文件 (public)
hexo clean

- 生成静态文件
hexo g（即hexo generate）

- 启动服务器：默认情况下，访问网址为：http://localhost:4000/。
hexo s（即hexo server）

- 一键部署
npm i hexo-deployer-git --save
hexo d（即hexo deploy）

- 文件生成后立即部署网站
hexo g -d