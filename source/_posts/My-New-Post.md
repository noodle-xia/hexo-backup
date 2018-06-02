---
layout: photo
title: vue-cli多页面脚手架
date: 2017-03-20 21:24:42
tags:
- vue
- 前端框架
- 随笔
category: 
- code
- 学习

---
 学习使用vue-cli多页面脚手架
<!-- more -->

## 关于vue-cli
`Vue-cli`是vue官方提供的一个命令行工具（vue-cli），可用于快速搭建大型单页应用。（之前体验学习`vue.js`一段时间，慢慢开始接触使用vue-cli多页面脚手架）。帮助你快速开始一个vue项目，其实其本质就是给你一套文件结构，包含基础的依赖库，你只需要`npm install`一下就可以安装。让你不需要为编译或其他琐碎的事情而浪费时间，这并不会限制到你的发挥。（看到有人好像是这么解释的，很赞同这个答案）
## 学习vue之旅
相关学习博客链接:[Vue2.0新手完全填坑攻略—从环境搭建到发布](https://segmentfault.com/a/1190000007124470) 
### 使用方法
```
# install dependencies
npm install

# serve with hot reload at localhost:8080/module/index.html
npm run dev   //运行

# build for production with minification
npm run build   //打包 
```
输入完命令`npm run dev`会自动启动浏览器，自动启动浏览器就会看到vue图标的界面了 如

![](http://onh2yw93k.bkt.clouddn.com/005.png)

`npm run build`是项目打包命令，运行这个命令后会生成可以进行上线的打包文件，这时候打开根目录（dist）下的index.html就可以直接看到你的项目效果了。
在使用 `atom` 编辑时进一步认识atom编辑器与`subline`的区别，另外在打开`IDE`这一项时，使用atom打开项目需要安装 Vue 语法高亮的插件，使项目代码可读性更好。添加插件方法：
在atom编辑页面选项栏中点击`Packages`，选择`Settings View `——> `Install Packages/Themes`,然后搜索需要添加的插件，如图：
![](http://onh2yw93k.bkt.clouddn.com/006.png)
### 随笔
哈哈 之前看博客教程里提到有需要填的坑，自己没在意，直接看下面的了，现在果然跳进去了，当自己试着打包别人做好的项目时，出现`cannot find module 'clean-webpack-plugin' `里面确实提醒了少哪个插件下哪个。。哈哈 
慢慢来。。加油！
- **下一步**
通过学习vue-cli多页面脚手架和别人的demo 尝试搭建自己的多页面个人主页