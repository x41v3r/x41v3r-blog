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

#### （1）meta元素

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

<!--每 5 秒刷新一下浏览器并跳转到指定页面-->
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
</head>
<body>
    <h1>header 1</h1>
    <p>A paragraph.</p>
    <a href="http://www.baidu.com" target="">好看的<a/>
</body>
</html>
```
*   type属性只能是"text/css"。
*   media属性用来表明文档在什么情况下应该使用该元素中定义的样式。
    *   all：将样式用于所有设备（默认）
    *   print：将样式用于打印机模式（**只在打印模式下才会应用该样式**）
    *   screen：将样式用于计算机屏幕
*   有多个style标签的情况下，默认未设置media属性的style标签设置的优先级低于设置了media属性的style标签，只有当其他各个设置了media属性的style标签的media条件都不符合时才会应用默认style标签的样式。






> 看到小甲鱼b站视频 《零基础入门学习Web开发》 p 6  
> 人的一切痛苦，本质上都是对自己的无能的愤怒。




### 2.img标签和a标签

#### （1）img标签

```html
<img alt="hi!" src="pics/picture.png" width="800px" height="500px" />
```
*   alt属性值：鼠标悬停在图片上方的显示内容
*   width和height属性表示用于设置图片的显示大小

#### （2）a标签

```html
<a href="https://baidu.com" target="_blank" >有问题，问百度</a>
```
*   href属性内容为一个url，跳转的目标
*   target属性表示点击超链接的动作
    *   _blank  在新标签页打开
    *   _self   在当前窗口打开（默认）
    *   











## 二、JavaScript

## 三、CSS

## Vue.js框架

