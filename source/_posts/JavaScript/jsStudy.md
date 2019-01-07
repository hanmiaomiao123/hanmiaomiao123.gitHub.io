---
title: jsContent
tags:
---
###
JavaScript实现
--
```
一个完整的JavaScript实现应该有下列三个不同的部分组成：
核心（ECMAScript）
文档对象模型DOM
浏览器对象模型BOM
```
```
ECMAScript 6（以下简称ES6）是JavaScript语言的下一代标准.
ECMAScript是JavaScript语言的国际标准，JavaScript是ECMAScript的实现。
```
#####
$符号的含义：
--
```
1. 变量的连接符 ，且并不可以用作地址引用     如$a1_2
2. 全局函数的应用：
   ① JQuery中$(document).xxx的用法：myFunc(document).xxxx是不是瞬间就看出了它的本质，所以$()这就是一个普通的函数，只不过在JQuery中把它定义了出来，而可以直接用。
   ②  然而对于不同js脚本，$()的功能也不同，你也可以在自己的框架中重写$()方法；
3. 定义js脚本的关键字变量
```
