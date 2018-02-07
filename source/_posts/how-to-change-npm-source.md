---
layout: post
catalog: true
title: npm换源
header-img: https://ws1.sinaimg.cn/large/77ce63b1gy1fjd88xw2mjj20qy0emdg3.jpg
date: 2017-09-09 13:12:32
tags:
	- npm
	- cnpm
---

## 换源
更换npm源地址
``` bash
npm config set registry https://registry.npm.taobao.org
```

检查npm原地址
``` bash
npm config get registry 
```
出现错误
``` bash
npm info retry will retry, error on last attempt: Error: CERT_UNTRUSTED
```

解决方法
``` bash
npm config set strict-ssl false
```

## cnpm代替npm
``` bash
npm install -g cnpm --registry=https://registry.npm.taobao.org
```