---
layout: post
title: HTML学习笔记-4.HTML 属性
category: project
description: HTML学习笔记_w3school
---

> * HTML 标签可以拥有属性。**属性为HTML 元素提供附加信息**。
* 属性总是以名称/值 对的形式出现，比如：`name="value"`。
* 属性总是在HTML元素的**开始标签**中规定。

##属性实例：

* **链接属性：**HTML 链接由`<a>`标签定义。链接的地址在`href` 属性中指定：

`<a href="http://www.baidu.com">百度一下，你就知道</a>`

* **标题属性：**`<h1>`定义标题的开始<br />`<h1 align="center">`拥有关于对其方式的附加信息。![](http://upload-images.jianshu.io/upload_images/1633880-5d056ffc6bcc166b.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* **页面颜色：**`<body>`定义HTML 文档的主体。<br />`<body bgcolor="green">`拥有关于背景颜色的附加信息。![](http://upload-images.jianshu.io/upload_images/1633880-cdf4bbae53e3fd49.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* **表格属性：**`<table>`定义HTML 表格。<br />`<table border="1">`拥有关于表格边框的附加信息。
##HTML提示
* **使用小写属性：**属性和属性值对**大小写不敏感**。<br />但是[万维网联盟](https://www.w3.org/)在其HTML 4 推荐标准中**推荐小写的属性/属性值**。<br />而新版本的(X)HTML 要求使用小写属性。
* **始终为属性值添加引号：**属性值应该始终被包括在引号内。双引号是最常用的，不过使用单引号也没有问题。<br />在某些个别的情况下，如属性值本身就含有双引号，那么必须使用单引号，例如：<br />`name='Jay "Hello World" F4n`

##HTML 属性参考手册
[**完整的HTML 参考手册**](http://w3school.com.cn/tags/index.asp)提供了每个HTML 元素可使用的合法属性的完整列表。<br />下面列出了使用大多数HTML 元素的属性：

| 属性    | 值                | 描述                      |
| ----- | ---------------- | ----------------------- |
| class | classname        | 规定元素的类名                 |
| id    | id               | 规定元素的唯一id               |
| style | style_definition | 规定元素的行内样式（inline style） |
| title | text             | 规定元素的额外信息（可在工具提示中显示）    |


更多关于标准属性的信息，请访问：

[**HTML 标准属性参考手册**](http://w3school.com.cn/tags/html_ref_standardattributes.asp)
