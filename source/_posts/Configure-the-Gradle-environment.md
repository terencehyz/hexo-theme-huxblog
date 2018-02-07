---
title: 配置Gradle环境
tags:
  - Gradle
date: 2017-09-17 10:47:15
layout: post
author: "Terence Han"
catalog: true
header-img: https://ws1.sinaimg.cn/large/77ce63b1ly1fjmhkn4istj21jk0p075d.jpg
---
## 下载Gradle
[下载地址：https://gradle.org/releases/](https://gradle.org/releases/)
> 下载 `binary-only`版本

## 配置环境
### Mac OS
本机存放地址为`/Users/terencehyz/gradle/gradle-4.1`
1. 打开终端(Terminal)并输入
``` bash
touch .bash_profile
```

2. 打开`.bash_profile`文件
``` bash
open .bash_profile
```
3. 在文件中输入
``` bash
GRADLE_HOME=/Users/terencehyz/gradle/gradle-4.1;
export GRADLE_HOME
export PATH=$PATH:$GRADLE_HOME/bin
```

4. 保存`.bash_profile`并执行
``` bash
source ~/.bash_profile
```
更新`.bash_profile` 文件

### Windows
1. 新建环境变量`GRADLE_HOME`为本地地址`D:\gradle-4.1`
2. 修改环境变量`PATH`，增加`%GRADLE_HOME%\BIN;`


## 检查配置是否成功
在终端（Mac OS）或（CMD）执行
``` bash
gradle -version
```
![](https://ws1.sinaimg.cn/large/77ce63b1ly1fji6fv9pxij20gb0ac757.jpg)

MacOS
![](https://ws1.sinaimg.cn/large/77ce63b1gy1fjmcj4qgicj20r90e9mx8.jpg)
Windows