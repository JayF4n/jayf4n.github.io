---
layout: post
title: HTML学习笔记-3.HTML 元素
category: project
description: HTML学习笔记_w3school
---

HTML 元素指的是从开始标签（start tag）到结束标签（end tag）的所有代码。

| 开始标签                   | 元素内容                | 结束标签 |
| ---------------------- | ------------------- | ---- |
| `<p>`                    | this is a paragraph | `</p>` |
| `<a href="default.htm"> `| this is a link      | `</a>` |
| `<br />`                |                     |      |

> **注释：**开始标签常被称为**开放标签**（opening tag）,结束标签常被称为**闭合标签**（closing tag）

---------------
##HTML 元素语法
* HTML 元素以**开始标签**起始
* HTML 元素以**结束标签**终止
* **元素的内容**是开始标签与结束标签之间的内容
* 某些 HTML 元素具有**空内容**（empty content）
* 空元素**在开始标签中进行关闭**（以开始标签的结束而结束）
* 大多数 HTML 元素可拥有属性

------------------------
##嵌套的 HTML 元素
大多数 HTML 元素 可以嵌套（可以包含其他 HTML 元素）。

HTML  文档由嵌套的 HTML 元素构成。

**HTML文档实例：**

    <html>
        <body>
        <p>this is my first paragraph.</p>
        </body>
    </html>

上面的例子包含三个 HTML元素。
**HTML 实例解释：**

**`<p>`元素**

    <p>this is my first paragraph.</p>

* 这个`<p>`元素定义了HTML 文档的一个段落。
* 这个元素拥有一个开始标签`<p>`和一个结束标签`</p>`。
* 元素的内容是：this is my first paragraph.

**`<body>`元素：**

    <body>
    <p>this is my first paragraph.</p>
    </body>

* `<body>`元素定义了HTML 文档的主体。
* 这个元素拥有一个开始标签`<body>`和一个结束标签`</p>`。
* 元素内容是另一个HTML 元素（`<p>`元素）。

**`<HTML>`元素：**

    <html>

        <body>
        <p>This is my first paragraph.</p>
        </body>

    </html>

* HTML 元素定义了整个HTML 文档。
* 这个元素拥有一个开始标签`<html>`和一个结束标签`</html>`。
* 元素内容是另一个HTML 元素（`<body>`元素）。

**不要忘记结束标签**
即使忘记了使用结束标签，大多数浏览器也会正确地显示HTML：

    <p>you forgot your end tag
    <p>hmm...i know it.
**但是永远不要忘记使用结束标签，因为会产生不可预料的结果或错误。未来的HTML 版本不允许省略结束标签。**

##空的 HTML 元素
*　没有内容的HTML 元素被称为空元素。空元素是在开始标签中关闭的。
*　`<br>`就是没有关闭标签的空元素（**`<br>`标签定义换行**）。
*　在 XHTML、XML 以及未来的HTML 中，所有元素都必须被关闭。
*　在开始标签中添加斜杠，比如`<br />`,是关闭元素的正确方法，HTML、XHTML、和 XML 都接受这种方式。即使`<br>`在所有浏览器中都是有效的，但是用`<br />`其实是更长远的保障。

##HTML 提示： 使用小写标签
HTML 标签对大小写不敏感：`<P>`等于`<p>`。许多网站都使用大写的HTML 标签。但是还是建议使用小写标签，因为[万维网联盟（W3C）](https://www.w3.org/) 在 HTML4 中**推荐**使用小写，而在未来(X)HTML 版本中**强制**使用小写。
