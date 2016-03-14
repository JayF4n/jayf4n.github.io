---
layout: post
title: HTML学习笔记-11.HTML表格
category: project
description: HTML学习笔记_w3school
---

## 表格

表格由`<table>`标签来定义。每个表格均有若干行（由`<tr>`标签定义），每行被分割为若干单元格（由`<td>`定义）。td（table data）可以包含文本、图片、列表、段落、表单、水平线、表格等。

    <table border="1">
    <tr>
    <td>名字</td>
    <td>职位</td>
    <td>备注</td>
    </tr>
    <tr>
    <td>张三</td>
    <td>职员</td>
    <td>此人很懒</td>
    </tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/table.jpg)

## 表格和边框属性

如果不定义边框属性，表格将不显示边框。（`border="0"`）

## 表格的表头

使用`<th>`标签进行定义。

大多数浏览器会把表头定义为粗体居中的文本：

    <table border="1">
    <tr>
    <th>名字</th>
    <th>职位</th>
    <th>备注</th>
    </tr>
    <tr>
    <td>张三</td>
    <td>职员</td>
    <td>此人很懒</td>
    </tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/th.jpg)

## 表格中的空单元格

对于没有内容的空单元格，一些浏览器可能无法显示出边框。为了避免这种情况，可以在空单元格中添加一个空格占位符：

    <table border="1">
    <tr>
    <th>名字</th>
    <th>职位</th>
    <th>备注</th>
    </tr>
    <tr>
    <td>张三</td>
    <td>职员</td>
    <td>此人很懒</td>
    </tr>
    <td>李四</td>
    <td>职员</td>
    <td>&nbsp;</td>
    <tr></tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/nbsp.jpg)

## 更多实例

垂直的表头

    <table border="1">
    <tr>
    <th>姓名</th>
    <td>张三</td>
    <td>李四</td>
    </tr>
    <tr>
    <th>职位</th>
    <td>职员</td>
    <td>职员</td>
    </tr>
    <tr>
    <th>备注</th>
    <td>此人很懒</td>
    <td>&nbsp;</td>
    </tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/thth.jpg)

带有标题的表格（caption）

    <h4>这个表格有一个标题，以及粗边框：</h4>
    <table border="6">
    <caption>职工情况表</caption>
    <tr>
    <th>名字</th>
    <th>职位</th>
    <th>备注</th>
    </tr>
    <tr>
    <td>张三</td>
    <td>职员</td>
    <td>此人很懒</td>
    </tr>
    <td>李四</td>
    <td>职员</td>
    <td>&nbsp;</td>
    <tr></tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/caption.jpg)

跨行或跨列的单元格

    <h4>横跨两列的单元格：</h4>
    <table border="1">
    <tr>
    <th>Name</th>
    <th colspan="2">Tel</th>
    </tr>
    <tr>
    <td>JayF4n</td>
    <td>110</td>
    <td>120</td>
    </tr>
    </table>
    <h4>横跨两行的单元格：</h4>
    <table border="1">
    <tr>
    <th>Name</th>
    <td>JayF4n</td>
    </tr>
    <tr>
    <th rowspan="2">Tel</th>
    <td>110</td>
    </tr>
    <tr><td>120</td></tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/col-row.jpg)

表格内的标签

    <table border="1">
    <tr>
      <td>
        <p>第一行</p>
        <p>第二行</p>
      </td>
      <td>有一个表格：
        <table border="1">
        <tr>
            <td>1</td>
            <td>3</td>
        </tr>
        <tr>
            <td>2</td>
            <td>4</td>
        </tr>
        </table>
      </td>
    </tr>
    <tr>
      <td>有一个列表：
      <ul>
        <li>apple</li>
        <li>banana</li>
        <li>peach</li>
      </ul>
      </td>
      <td>有一个链接：
      <a href="jayf4n.github.io">JayF4n的Blog</a>
      </td>
    </tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/td-tags.jpg)

单元格边距（Cell padding）单元格间距（Cell spacing）

    <table border="1" cellpadding="10">
    <tr>
    <th>名字</th>
    <th>职位</th>
    <th>备注</th>
    </tr>
    <tr>
    <td>张三</td>
    <td>职员</td>
    <td>此人很懒</td>
    </tr>
    </table>
    <table border="1" cellspacing="10">
    <tr>
    <th>名字</th>
    <th>职位</th>
    <th>备注</th>
    </tr>
    <tr>
    <td>张三</td>
    <td>职员</td>
    <td>此人很懒</td>
    </tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/spadding-spacing.jpg)

表格添加背景

    <table border="1" bgcolor="pink">
    <tr>
    <th>名字</th>
    <th>职位</th>
    <th>备注</th>
    </tr>
    <tr>
    <td>张三</td>
    <td>职员</td>
    <td>此人很懒</td>
    </tr>
    </table>
    <table border="1" background="http://7xrabv.com1.z0.glb.clouddn.com/0312_1.png">
    <tr>
    <th>名字</th>
    <th>职位</th>
    <th>备注</th>
    </tr>
    <tr>
    <td>张三</td>
    <td>职员</td>
    <td>此人很懒</td>
    </tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/table-bg.jpg)

单元格添加背景

    <table border="1" >
    <tr>
    <th bgcolor="pink">名字</th>
    <th>职位</th>
    <th>备注</th>
    </tr>
    <tr>
    <td>张三</td>
    <td>职员</td>
    <td background="http://7xrabv.com1.z0.glb.clouddn.com/0312_1.png">
    此人很懒</td>
    </tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/cell-bg.jpg)

在单元格中排列内容

[W3school实例](http://w3school.com.cn/tiy/t.asp?f=html_table_align)

框架（frame）属性

    <h4>table with frame="box"</h4>
    <table frame="box">
    <th><td>All  man  must die</td></th>
    <tr><td>All  man  must server</td></tr>
    </table>
    <h4>table with frame="above"</h4>
    <table frame="above">
    <th><td>All  man  must die</td></th>
    <tr><td>All  man  must server</td></tr>
    </table>
    <h4>table with frame="below"</h4>
    <table frame="below">
    <th><td>All  man  must die</td></th>
    <tr><td>All  man  must server</td></tr>
    </table>
    <h4>table with frame="hsides"</h4>
    <table frame="hsides">
    <th><td>All  man  must die</td></th>
    <tr><td>All  man  must server</td></tr>
    </table>
    <h4>table with frame="vsides"</h4>
    <table frame="vsides">
    <th><td>All  man  must die</td></th>
    <tr><td>All  man  must server</td></tr>
    </table>

![](http://7xrabv.com1.z0.glb.clouddn.com/table-frame.jpg)

![](http://7xrabv.com1.z0.glb.clouddn.com/table-frame1.jpg)
