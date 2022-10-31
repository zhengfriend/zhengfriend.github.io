---
title: 如何将Hexo博客源码备份到github
tags: hexo
abbrlink: hexo02/
date: 2022-10-31 09:34:35

sticky: 9
toc_number: true
toc: true
cover: /custom/source/img/fengjing/fengjing5.jpg

---

# 前言
在前面的文章中，已经介绍了如何使用hexo 和 github 结合起来搭建个人博客了，
hexo d 部署到github上的文件其实只有 .deploy_git目录下的网页文件，不包含我们博客的源码的。
对于博客源码，比如source文件夹、配置文件等，我们可以利用git来做分支管理，对源码进行备份，这样，
我们就可以在另一台电脑或其他环境上把源码clone到本地，然后经过环境配置后，就可以继续写我们的博客了。

# Hexo博客源码备份

# 创建hexo分支
在github上，博客仓库下，创建一个新的分支，blog-hexo ， 并将这个分支设置为默认分支。

![20221031_01](/custom/source/blogimg/20221031/20221031_01.png)
![20221031_02](/custom/source/blogimg/20221031/20221031_02.png)


# 克隆hexo分支
* 在本地创建一个新目录，然后把刚新建的分支克隆到这个目录下
* 吧克隆下来的项目里面的.git文件夹，复制到我们的博客根目录下；

注意：如果之前搭建博客的时候，自己更换过主体文件的，请把主体文件里面的 .git 目录删除。

# 开始备份
进入到bolgs根目录，执行如下命令：
```bash
git add .
git commit -m "Blog源文件备份"
git push origin blog-hexo
```
这时候，我们在github上的blog-hexo就有我们的源文件了。

如果你想每次更改东西都希望备份到blog-hexo分支上，可以执行如下步骤：
```bash
hexo clean
git add .
git commit -m "备份"
git push
hexo g 
hexo d
```

# 如何恢复博客

假如我们更换了电脑，或者想要在新的目录下重新构建博客，把github上的blog-hexo分支克隆到本地
进入到克隆先来的目录下，执行如下命令：
```bash
npm install hexo-cli
npm install hexo-deployer-git
```
然后再去安装主题相关的插件即可，当然如果你电脑上还没有node.js等环境的话，还需要安装相关的环境。

# 最后
到这里，如何备份Hexo博客源码以及如何回复Hexo博客源码就结束了。
更多关于Hexo框架和butterfly主题配置可以浏览博主相关文章。














