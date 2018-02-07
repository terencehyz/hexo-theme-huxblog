---
layout: post
title: Hosts
catalog: true
date: 2017-07-15 17:06:17
header-img: https://ws1.sinaimg.cn/large/77ce63b1ly1fhko6e6lsbj20p00dwjrn.jpg 
author: "TerenceHan" 
tags:
	- hosts

---
# 什么是hosts?
Hosts是一个没有扩展名的系统文件，可以用记事本等工具打开，其作用就是将一些常用的网址域名与其对应的IP地址建立一个关联“数据库” ，当用户在浏览器中输入一个需要登录的网址时，系统会首先自动从Hosts文件中寻找对应的IP地址，一旦找到，系统会立即打开对应网页，如果没有找到， 则系统再会将网址提交DNS域名解析服务器进行IP地址的解析。

# 为什么需要host?
G~F~W针对某些域名进行DNS污染，所以使我们无法解析到一个“正确”的IP地址。所以为了能够科学上网，我们便可以通过更改host的方法来完成。

# hosts文件从哪里来？
* [GitHub](https://github.com/search?utf8=%E2%9C%93&q=hosts&type=)中有较多开源项目
* [老D的Hosts](https://laod.cn/hosts/2017-google-hosts.html)
* [Merge-Public-Hosts](http://hosts.hanyuzhou.com/)
* ...

# hosts在哪里修改
* Windows 系统hosts位于 C:/Windows/System32/drivers/etc/hosts
* Android 系统hosts位于 /system/etc/hosts
* Linux 系统hosts位于 /etc/hosts
* Mac 系统hosts位于 /etc/hosts
* iOS 系统hosts位于 /etc/hosts

# 本站提供的hosts文件
Hosts内容合并自GitHub四个项目，可以满足基本使用。
> AD(vokins)：https://raw.githubusercontent.com/vokins/yhosts/master/hosts
play ： https://raw.githubusercontent.com/sy618/hosts/master/p
YouTube ： https://raw.githubusercontent.com/sy618/hosts/master/y
fq(racaljk)：https://raw.githubusercontent.com/racaljk/hosts/master/hosts

## 文件地址
[hosts.hanyuzhou.com](https://hosts.hanyuzhou.com)
