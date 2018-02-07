---
layout: post
title: 关于vue-cli
date: 2017-03-05 09:38:52
author: "TerenceHan"
header-img: https://ws1.sinaimg.cn/large/77ce63b1ly1fdbqj3h8poj21ig0qowfj
tags:
	- vue.js
	- vue-cli
	- JavaScript
---
## 安装
```
npm install -g vue-cli  
vue init webpack project-name
cd project-name
npm install   
npm run dev
```
> 注释    
`ESLint` ES6代码检查器    

## 项目文件
`build`和`config`都是webpack配置相关
`node_modules`是`npm install`安装的以依赖码库
`src`存放原码
`static`存放第三方静态资源
`.babelrc`将ES6编译成ES5
`editorconfig`编辑器的配置
