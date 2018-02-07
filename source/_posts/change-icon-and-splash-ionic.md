---
layout: post
catalog: true
title: ionic 2 ionic 3更换icon和splash
author: "TerenceHan"
header-img: https://ws1.sinaimg.cn/large/77ce63b1gy1fhyjztvqz5j20sg0g9aj5.jpg
date: 2017-07-27 16:40:58
tags:
	- ionic
---
### 准备工作
1. 工程中需要添加Androin或iOS平台
2. icon和splash图像文件
> icon图像最小尺寸为192×192px，非圆角图片。
splash图像最小尺寸为2208×2208px。
图像格式支持.png、.psd、.ai
icon文件命名为icon.png
splash文件命名为splash.png

### 操作步骤
1. 删除resource文件夹下android文件夹和iOS文件夹。
2. 进行终端操作

```
ionic resource  //同时修改icon和splash
```
```
ionic resource --icon   //只修改icon
```
```
ionic resource --splash //只修改splash
```