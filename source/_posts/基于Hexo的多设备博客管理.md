---
title: 基于Hexo的多设备博客管理
date: 2022/6/17
tags:
- Hexo
categories:
- programmer
---


## Hexo机制
Hexo部署到GitHub上面的只有`.deploy_git`文件夹内的静态文件，原始文件仍在本地`blog`文件夹中。


<!--more-->


## 操作步骤（未有博客）
```
# 创建本地blog文件夹，同步到GitHub。

# 在Github仓库新建hexo分支，并将其设置为默认分支。

# git clone git@github.com:loganjin/loganjin.github.io.git到本地电脑，删除除.git文件夹外全部文件。  
attention: 因为默认分支已经设成了hexo分支，所以clone时只clone了hexo分支，clone这个空仓库是为了其中隐藏的.git文件夹，从而达到通过git操作hexo分支管理博客文件的目的。

#将.git文件夹复制到本地blog文件夹。

这样就可以通过main分支管理静态文件(hexo操作)，hexo分支管理博客文件(git操作)。

attention: 由于git不能嵌套上传，如果存在git clone主题操作，应该将themes文件夹内的.git文件夹删除。
```


## 操作步骤（已有博客）
```
# 在Github仓库新建hexo分支，并将其设置为默认分支。

# git clone git@github.com:loganjin/loganjin.github.io.git到本地电脑，生成loganjin.github.io文件夹。

# 在本地loganjin.github.io文件夹下依次执行npm i hexo-cli -g、npm install和npm i hexo-deployer-git --save。  
attention: 此时如果使用hexo init，会初始化博客，最外层的_config.yml文件会恢复成默认值，新生成的.git文件夹会覆盖我们需要的.git文件夹。

# 修改_config.yml中的deploy参数为main。

这样就可以通过main分支管理静态文件(hexo操作)，hexo分支管理博客文件(git操作)。
```
