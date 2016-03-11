---
layout: post
title: Github Pages 建立个人博客总结
category: blog
description: 折腾一下Github pages。
---

> **参考[Beiyun](http://beiyuu.com/)的文章[使用Github Pages建独立博客](http://beiyuu.com/github-pages/)。**

## 配置Github

这里我直接使用了[GithubDesktop](https://desktop.github.com/)客户端，安装登录之后关于SSH Key的部分会自动完成，不过Git的帐号信息还是要设置一下：

    $ git config --global user.name "你的名字"
    $ git config --global user.email "your_email@youremail.com"


名字和邮箱替换成自己的，Github会用这些信息做相关权限的处理。

## 使用Github Pages 新建项目

> 在这步我折腾了好久，建立项目上传之后，[jayf4n.github.io](jayf4n.github.io)一直显示404，最后发现是弄成了依附于项目的pages。


1. 登录Github网站，点击`+New repository` ，项目名称为`username.github.io` ,这里的username必须是Github账号的用户名。

2. 在Github Desktop 里将刚才的项目克隆到本地。打开 Git shell：

进入项目目录

    cd username.github.io                 #进入项目目录

在本地的项目目录里添加index.html文件

    git add index.html                     #将index.html文件添加到暂存区
    git commit -a -m "First pages commit"  #将暂存区的修改提交到当前分支
    git push                               #将修改同步到Github
可以打开`username.github.io`开下是否成功
![](http://7xrabv.com1.z0.glb.clouddn.com/first-commit.jpg)

## 套用Jekyll模板

> 这里我folk了[Beiyun](http://beiyuu.com/)的[模板](https://github.com/beiyuu/Github-Pages-Example)。

1. 下载模板，可以在客户端里下载也可以在Git shell用`git clone https://github.com/beiyuu/Github-Pages-Example `命令。

2. 删除之前的index.html文件，在Git shell里打开

    `git rm index.html`
    `git commit -m "delete first-pages"`

将除了**.git**文件夹的所有内容复制到自己的user.github.io文件夹内。

3. 修改模板，将里面关于社交资料的内容改为自己的。删除images和_posts文件夹里的内容,原作者用的是本地图片在Git里上传，我自己在Markdwon链接的是[七牛云存储](https://portal.qiniu.com/)的图床。

4. 加入自己的文章，md文件命名格式为year-month-day-title.md，例如2016-03-06-github-pages.md，放到_posts文件夹里对应的分类中。

> **YAML Front Matter和模板变量**

>对于使用YAML定义格式的文章，Jekyll会特别对待，他的格式要求比较严格，必须是这样的形式：

    ---
    layout: post
    title: Blogging Like a Hacker
    ---
> 前后的---不能省略，在这之间，你可以定一些你需要的变量，layout就是调用_layouts下面的某一个模板，他还有一些其他的变量可以使用：

> `permalink` 你可以对某一篇文章使用通用设置之外的永久链接
> `published`可以单独设置某一篇文章是否需要发布
> `category` 设置文章的分类
> 上面的title就是自定义的内容，你也可以设置其他的内容，在文章中可以通过`{ { page.title }}`这样的形式调用。

>还有其他需要的变量，可以参考[官方的文档](https://github.com/mojombo/jekyll/wiki/template-data)

![](http://7xrabv.com1.z0.glb.clouddn.com/gitpages.jpg)

## 同步到Github pages

    cd username.github.io                   #进入目录
    git add .                               #添加修改到暂存区
    git commit -m "add Beiyunn's theme"     #添加修改到当前分支
    git push                                #将修改同步到Github

完成之后可以在浏览器里看下是否成功

主页
![](http://7xrabv.com1.z0.glb.clouddn.com/index.jpg)

文章
![](http://7xrabv.com1.z0.glb.clouddn.com/blog.jpg)

> 至此利用Github pages和Jekyll模板搭建个人博客已经完成了，接下来就是不断学习与完善了;_)

## Git与Markdown教程

* **Git教程推荐[史上最浅显易懂的Git教程！_廖雪峰](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)**
* **Markdown请看[Markdown_维基百科](https://zh.m.wikipedia.org/wiki/Markdown)**

