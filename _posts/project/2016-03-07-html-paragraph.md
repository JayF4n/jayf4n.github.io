---
layout: post
title: HTML学习笔记-6.HTML段落
category: project
description: HTML学习笔记_w3school
---

## HTML段落

HTMl段落是通过`<p>`标签定义的。

    <p>what i got to do to make you love me </p>
    <p>what i got to do to make you care</p>

> 浏览器会自动在段落的前后添加空行（`<p>`是块级元素）
> 插入空行不要使用`<p></p>`，应该使用`<br />`
> 不要忘记结束标签`</p>`


## 段落内拆行

使用`<br />`标签
说到拆行，就不得不提到赵老师的梨花体了= =！:

    <html>
        <body>
        <h4 align="center">我坚决不能容忍</h4>
        <p>我坚决不能容忍<br />那些<br />在公共场所<br />的卫生间<br />大便后<br />不冲刷<br />便池<br />的人</p>
        </body>
    </html>
由于Markdown是兼容HTML格式的，我们可以将代码块的标识去掉，那么就可以看到上面的代码在浏览器里呈现的效果了：
<html>
        <body>
        <h4 align="center">我坚决不能容忍</h4>
        <p>我坚决不能容忍<br />那些<br />在公共场所<br />的卫生间<br />大便后<br />不冲刷<br />便池<br />的人</p>
        </body>
</html>

> 我竟无言以对，看来梨花题叫作`<br />体`也行嘛。。


## 小结

* 换行尽量使用`<br />`

* 浏览器会移除代码中多余的空格与换行，代码里所有连续的空格/空行/ 均被显示为一个空格，但是连续的`<br />`会正确的实现,于是梨花体变成了查看全文体:
![](http://7xrabv.com1.z0.glb.clouddn.com/br.jpg)
