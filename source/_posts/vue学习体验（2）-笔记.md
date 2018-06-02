---
title: vue学习体验（2）-笔记
date: 2017-03-13 22:29:40
tags:
- vue
- 前端框架
category: code

---
之前练习了一些从模型数据到视图的单向绑定，这次运用 v-model指令实现视图到模型的一个传递，依然结合jQuery的一些实现方法进行比较，加深自己的理解。
<!-- more -->
**代码部分：**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>02</title>
</head>
<body>
<div id="app">
    <input type="text" v-model="msg"> <!--显示input输入的内容-->
    <h1>{{msg}}</h1>
</div>

<!--<script type="text/javascript" >  -->
<!--//用jqury实现要达到的需求-->
<!--//$('input').on('keydown',function (e) {   -->
    <!--//在jQuery中获取input元素-->
    <!--//其他获取方式  1、this 2、e.target    -->
<!--//    console.log(e.target)-->
    <!--//获取Input的值 var val=e.target.value   -->
<!--//    var val =$(this).val();  -->
<!--// 或者   $('h1'').html(val)   -->
<!--})-->
<script src="vue.js"></script>
<script type="text/javascript">
var app=new Vue({
   el:'#app',
   data:{
       msg:'0922'
   }
})
</script>
</body>
</html>
```
**理解及总结：** 
  开始练习了一些是模型数据通过vue的data属性实现数据到vue的一个绑定，此时数据更新会被vue监听渲染给视图，现在运用的`v-model`指令则是实现了视图到vue实例化对象的一个数据传递，假若视图更新，vue就会捕捉到，就会传递给模型数据。
（`v-model`的属性值是一个js作用域，也就是一个js环境，在其中添加属性值就是添加Vue实例化对象的变量。有点绕口。。。。哈哈哈）