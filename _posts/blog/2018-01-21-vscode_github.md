---
layout: post
title: VSCode与Github实现同步
category: blog
description: VScode与Github同步的设置。
---

## 设置Git的用户信息，生成公钥

[Git](https://git-scm.com/)的安装这里就不再赘述了，安装完成之后需要配置Git的账户信息，在Gitbash中输入以下信息：
```
//将用户名与邮箱替换成自己的即可
$ git config --global user.name "your_name"
$ git config --global user.email "your_email@youremail.com"
```
这里我使用的是Win7的系统，右键选择`Gitbash Here`,使用`SSH-keygen`命令生成密钥对：
```
ssh-keygen -t rsa -C"your_email@youremail.com"
```
密钥生成路径选择默认，密码可以留空，这样连接的时候就不需要输入密码了,在`/c/Users/你的用户名/.ssh/`文件夹下会生成一对密钥：
```
id_rsa         //私钥
id_rsa.pub     //公钥
```
## Github中设置公钥信息

在Gihub个人界面的`Personal settings--SSH and GPG keys`中添加SSH key，将刚才生成的id_rsa.pub中的内容复制即可。
测试连接是否成功，在Gitbash中使用如下命令：
```
$ ssh -T git@github.com
```
```
Hi JayF4n! You've successfully authenticated, but GitHub does not provide shell access.
```
可以看到连接成功的欢迎信息，Github不提供使用shell连接SSH的功能。

## VScode的目录与Github的项目进行连接

第一次使用[VScode](https://code.visualstudio.com/)需要设置Git的路径，在文件-首选项-设置里添加：
```
 "git.path": "E:/Programs/Git/bin/git.exe"  //这里自行替换自己的Git路径
```
在Github页面中新建一个repository，这里我新建了一个项目取名为test，在VScode中打开命令面板输入：
```
git clone
```
回车后输入项目的地址：
```
https://github.com/JayF4n/test
```
然后选择本地存储路径即可完成VScode与Github的连接，可以通过VScode的命令面板或者GUI执行Git的各项操作并同步发布到Github。