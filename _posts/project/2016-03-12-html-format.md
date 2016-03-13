---
layout: post
title: HTML学习笔记-7.HTML格式化
category: project
description: HTML学习笔记_w3school
---

## 文本格式化


    <html>
        <h1 align="center">米店</h4>
        <body>
        <!--标题居中-->
        <small>窗外的人们 匆匆忙忙</small>
        <!--定义小号字体-->
        <hr />
        <i>把眼光丢在潮湿的路上</i>
        <!--定义斜体字-->
        <hr />
        你的舞步 划过空空的<sub>房间</sub>
        <!--定义下标字
        <hr />
        时光就变成<sup>了烟</sup>
        <!--定义上标字-->
        <hr />
        <b>爱人 你可感到明天已经来临</b>
        <!--定义粗体文本-->
        <hr />
        <strong>码头上停着我们的船 </strong>
        <!--定义强调语气-->
        <hr />
        <big>我会洗干净头发 爬上桅杆</big>
        <!--定义大号字体-->
        <hr />
        <em>撑起我们葡萄枝嫩叶般的家</em>
        <!--定义着重文字-->
        </body>
    </html>



![](http://7xrabv.com1.z0.glb.clouddn.com/wb.jpg)





## 预格式文本`<pre>`



    <html>

    <body>
    <pre>
    这是
    预格式文本。
    它保留了      空格
    和换行。
    </pre>
    <p>pre 标签很适合显示计算机代码：</p>

    <pre>
    for i = 1 to 10
     print i
    next i
    </pre>

    </body>
    </html>




![](http://7xrabv.com1.z0.glb.clouddn.com/pre.jpg)





## “计算机输出”标签





    <html>

        <body>

        <code>Computer code</code>
        <!--定义计算机代码-->
        <br />
        <kbd>Keyboard input</kbd>
        <!--定义键盘码-->
        <br />
        <tt>Teletype text</tt>
        <!--定义打字机代码-->
        <br />
        <samp>Sample text</samp>
        <!--定义计算机代码样本-->
        <br />
        <var>Computer variable</var>
        <!--定义变量-->
        <br />

        <p>
        <b>注释：</b>这些标签常用于显示计算机/编程代码。
        </p>

        </body>
    </html>



![](http://7xrabv.com1.z0.glb.clouddn.com/code.jpg)




## 地址`<address>`




    <html>
     <body>
        <address>
        Written by <a href="mailto:jayf4n@gmail.com">Jay F4n</a>.<br>
        Visit us at:<br>
        jayf4n.gitbub.io<br>
        Box 564, Beijing<br>
        CHINA
        </address>
     </body>
    </html>




![](http://7xrabv.com1.z0.glb.clouddn.com/addressjpg.jpg)



## 文字方向`<bdo>`



    <html>
      <body>
        <p>
        如果您的浏览器支持 bi-directional override (bdo)，下一行会从右向左输出 (rtl)；
        </p>
        <bdo dir="rtl">
        Here is some Hebrew text
        </bdo>
        <!--定义文字方向-->
      </body>
    </html>



![](http://7xrabv.com1.z0.glb.clouddn.com/bdo.jpg)




## 块引用




    <html>
        <body>
            这是长的引用：
            <blockquote>
            这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的       引用。这是长的引用。这是长的引用。这是长的引用。
            </blockquote>
            这是短的引用：
            <q>
            这是短的引用。
            </q>
            <p>
            使用 blockquote 元素的话，浏览器会插入换行和外边距，而 q 元素不会有任何特殊的呈现。</p>
        </body>
    </html>




![](http://7xrabv.com1.z0.glb.clouddn.com/quote.jpg)





## 删除字和插入字



    <html>
      <body>
        <p>一打有 <del>二十</del> <ins>十二</ins> 件。</p>
        <p>大多数浏览器会改写为删除文本和下划线文本。</p>
        <p>一些老式的浏览器会把删除文本和下划线文本显示为普通文本。</p>
      </body>
    </html>




![](http://7xrabv.com1.z0.glb.clouddn.com/del.jpg)



-------------------------



文本格式化标签

* `<b>`  : 定义粗体文字

* `<big>` : 定义大号字体

* `<em>` : 定义着重文字

* `<i>` : 定义斜体字

* `<small>` : 定义小号字体

* `<strong>` : 定义加重语气

* `<sub>` : 定义下标字

* `<sup>` : 定义上标字

* `<ins>` : 定义插入字

* `<del>` : 定义删除字



“计算机输出”标签

* `<code>` : 定义计算机代码

* `<kbd>` : 定义键盘码

* `<samp>` : 定义计算机样本代码

* `<tt>` : 定义打字机代码

* `<var>` : 定义变量

* `<pre>` : 定义预格式文本


引用、引用和术语定义

* `<abbr>` : 定义缩写

* `<acronym>` : 定义首字母缩写

* `<address>` : 定义地址

* `<bdo>` : 定义文字方向

* `<blockquote>` : 定义长的引用

* `<q>` : 定义短的引用语

* `<cite>` : 定义引用、引证

* `<dfn>` : 定义一个项目















































































