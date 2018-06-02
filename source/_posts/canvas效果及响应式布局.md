---
title: canvas效果及响应式布局加深理解
date: 2017-04-20 13:18:03
tags:
- canvas
- demo
- 随笔

category:
- 响应式
- 随笔

---
![](http://onh2yw93k.bkt.clouddn.com/cloud.gif)
——温故而知新
<!--more-->
##### 温故
`<canvas></canvas>`标签像所有的dom对象一样它有自己本身的属性、方法和事件，其中就有绘图的方法，js能够调用它来进行绘图。
```
 var context =canvas.getContext("2d");
```
代码中`context`是一个封装了很多绘图功能的对象，2d则是提供2d动画效果，同样使用`webgl`可以实现`3d`效果。
canvas元素绘制图像的时候常用两种基本方法：
```
context.fill()//填充
context.stroke()//绘制边框
```
颜色的应用使用十六进制颜色值`#fff`等，也可直接使用颜色名称，还有
```
rgb(1-255,1-255,1-255)
rgba(1-255,1-255,1-255,0.1-0.9 //透明度)
```
在我设置移动端导航页面应用到。
###### 使用 HTML5 Canvas标签 画一个简单的时钟
几个月之前开始学习时，学着画一个简单的时钟来练手，利用`canvas`使用` JavaScript `在网页上绘制图像，先构造一个画布，画布是一个矩形区域，可以控制其每一像素。代码和`demo`上传在前端小屋的笔记，可进行效果预览 [使用 HTML5 Canvas标签 画一个简单的时钟](http://www.qdfuns.com/notes/42658/81fd0ba1c33652b5ecaa45faa21570de.html)
###### Canvas为网页添加动态背景 
我的移动端主页参考：








##### 知新
