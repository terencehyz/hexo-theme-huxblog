---
layout: post
title: vue.js移动设备开发技巧
date: 2017-03-05 09:40:58
author: "TerenceHan"
header-img: https://ws1.sinaimg.cn/large/77ce63b1ly1fdbqj3h8poj21ig0qowfj
tags:
	- vue.js
	- JavaScript
	- iOS
	- Android
---
## 样式
### 三栏布局

```javascript
.tab{
    display: flex;
    width: 100%;
    height: 40px;
    line-height: 40px;
}
.tab .tab-item{
	flex: 1;
    text-align: center;
}
```
对于`<a>`可以设置`display: block`从而实现点击某一块即可进行跳转
