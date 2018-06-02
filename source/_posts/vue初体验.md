---
title: vue初体验
date: 2017-03-09 20:29:35
tags: 
- 前端框架
- vue
category: code
 
---
简单的学习了一点Vue（mvvm模型），通过与原生js和jQuery写法相比较体验Vue的方便，条理清晰，不会使项目显得杂乱。实现数据到视图的双向绑定。
<!-- more -->
  代码部分：
```
---
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>01</title>
        <script src="jquery-3.1.1.min.js"></script>
        <script src="vue.js"></script>
    </head>
    <body>
    <div id="a">{{msg}}</div>
    <script type="text/javascript">
        var data ={
            msg:"你绝望了么？？"
        }
        data.msg="致胜一击 只要心够决！！"
    //    data.msg="致胜一击 只要心够决！！"
    //    document.getElementById("a").innerHTML=data.msg;
        //原生js写法。。
    //    document.getElementById("a").innerHTML=data.msg;
    //    $("#a").html(data.msg).html(data.msg)
        //jQury写法。。
        //创建vue实例化对象，（vm对象——绑定视图和数据..）
    new Vue({
       //绑定视图
      el:"#a",
       //绑定数据
       data:data,
   })
        data.msg="致胜一击 只要心够决！！"
    </script>
    </body>
    </html>
---
```