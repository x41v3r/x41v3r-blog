# Web前端开发

## 一、HTML5

> 超文本标记语言 **版本5**

### 1.第一个程序

```html
<!DOCTYPE html>
<html>
    <head>
        <title>第一个程序</title>
    </head>
    <body>
        <h1>hello,world</h1>
        <p>hello,html!</p>
    </body>
</html>
```
*   说明：
    *   head标签用以定义文档的头部，它是所有头部元素的容器
    *   title元素默认成为网页的链接内容
    *   body元素包含文档的主体内容

### 2.基础

#### （1）meta标签

```html
<!--指定字符集为UTF-8，防止乱码-->
<meta charset="UTF-8">

<!--设置网页尺寸自适应屏幕大小-->
<meta name="viewport" content="width=device-width,initial-scale=1.O">

<!--为搜索引擎提供关键词-->
<meta name="keywords" content="励志,改变,人生,未来">

<!--描述网页内容-->
<meta name="description" content="人生励志，不断激励，成为更好的自己">

<!--定义网页的作者-->
<meta name="author" content="x41v3r">

<!--打开 5 秒后刷新一下浏览器并跳转到指定页面-->
<meta http-equiv="refresh" content="5;http://www.baidu.com">
```
*   meta标签永远位于head标签内部。
*   content 属性必须和 name 或 http-equiv 属性共存亡。
*   

#### （2）style标签

```html
<html>
<head>
    <meta charset="UTF-8">
    <title>html5的style标签实例</title>
    <style type="text/css">
        h1 {color: red}
        p {color: blue}
    	a {
		    color: yellow;
			background: black;
		}
    </style>
    <style type="text/css" media="print">
        h1 {color: black}
        p {color: black}
    	a {
		    color: blue;
			background: black;
		}
    </style>
</head>
<body>
    <h1>header 1</h1>
    <p>A paragraph.</p>
    <a href="http://www.baidu.com" target="">这里有好康的！<a/>
</body>
</html>
```
*   type属性只能是"text/css"。
*   media属性用来表明文档在什么情况下应该使用该元素中定义的样式。
    *   all：将样式用于所有设备（默认）
    *   print：将样式用于打印机模式（**只在打印模式下才会应用该样式**）
    *   screen：将样式用于计算机屏幕
*   如果要使用media属性，那么我们需要将正常浏览模式下的style的media属性设置为screen（不可以不写），并将此style标签放在各个style标签的最后。

#### （3）base标签

> base标签用来设置一个基准 URL，让 HTML 文档中的相对链接在此基础上进行解析。

```html
<!--为body内使用相对路径a标签提供基准url-->
<base href="http://www.bilibili.com" target="_blank">

<!--使用相对路径的a标签，以base标签内的url为基准-->
<a href="/video/BV1D24y1X7TV">程女士</a>

<!--不使用相对路径的a标签，不受base标签内部url的影响-->
<a href="http://www.baidu.com">百度一下</a>
```
*   base必须放在head标签内
*   只影响同一个文件内使用相对路径的a标签，不影响使用绝对路径的a标签

### 3.图片

#### （1）area标签

#### （2）img标签

```html
<img alt="hi!" src="pics/picture.png" width="800px" height="500px" />
```
*   alt属性值：鼠标悬停在图片上方时显示的内容
*   src属性填写目标图片相对于当前html文件的相对路径
*   width和height属性用于设置图片的显示像素大小
*   

#### （3） 

### 4.链接

#### （1）a标签

```html
<a href="https://baidu.com" target="_blank" >有问题，问百度</a>
```
*   href属性内容为一个url，跳转的目标
*   target属性表示点击超链接的动作
    *   _blank  在新标签页打开
    *   _self   在当前窗口打开（默认）
    *   

#### （2）link标签

```html
<!--连接外部样式表-->
<link rel="stylesheet" type="text/css" href="css/style_file.css">

<!--链接网页图标-->
<link rel="icon" type="image/x-icon" href="img/site-icon.ico">
```
*   rel属性置为"stylesheet"链接外部样式表时，可以使用style标签的media属性。
*   

## 二、CSS

## 三、JavaScript

## Vue.js框架





> 看到小甲鱼b站视频 《零基础入门学习Web开发》 p 7
> 人的一切痛苦，本质上都是对自己的无能的愤怒。