---
title: LaTeX入门
tags:
  - LaTeX
date: 2018-01-26 23:23:08
layout: post
author: "TerenceHan"
header-img: https://ws1.sinaimg.cn/large/77ce63b1ly1fnvkj3lxn6j21ig0qo0v3.jpg
catalog: true
keywords: latex,latex入门
---

## 关于`\`
`\begin{环境名字}\end{环境名字}`是环境，用`\`开头，控制排版
`\document`,`\usepackage`是命令

## document环境中的写作
编辑器段与段之间要空一行，从而保证文本分段。
关于字体的命令/环境
1. 加粗 `\textbf{内容}`
2. 字号 `\normal` `\large` `\Large` `\LARGE` `\huge` `Huge`
> 字号大小在一个环境内或`{}`间生效    
例`{\large 123}`
3. 居中
```
\begin{center} 
内容 
\end{center}
```
4. 文章标题与作者、日期
`\title{标题名}`
`\author{作者名}`
`\date{日期}`
`\maketitle`
>`\maketitle`用于显示标题、作者、日期
5. 章节划分
`\section{章节名}`一级章节
`\subsection{章节名}`二级章节
`\subsubsection{章节名}`三级章节
6. 添加目录
`\tableofcontents`
7. 摘要环境
```
\begin{abstract}
摘要内容
\end{abstract}
```
8. 罗列环境
```
\begin{itemize}
\item    
\item    
\end{itemize}
```

## 关于公式
* 公式环境
1. 不可换行
```
\begin{equation}
公式    
\end{equation}
```

2. 可换行
```
\begin{algined}
& 公式\\
& 公式
\end{algined}
```
    >`&`用于对齐，`\\`用于换行  

3. 无编号公式
```
\begin{equation*}
公式
\end{equation*}
```
    或    
```
\begin{equation}\nonumber
公式
\end{equation}
```
    或`$$公式$$`    
    或`\[ 公式 \]`
4. 行内公式
`$公式$`
5. 公式命令
幂 `x^{2a+1}`
下标 `x_{2a+1}`
分式`\frac{x}{y}`
积分号`\int^{上限}_{下限}`
微分号`\mathrm{d}`
求和`\sum^{5}_{0}`
6. 大型公式(需要包含宏包mathtools)
矩阵
```
\begin{equation}
A=\begin{bmatrix}
    1&2 \\
    4&5
    \end{bmatrix}
\end{equation}
```

    大括号
```
\begin{equation}
\left\{
    \begin{aligned}
        & x^{2}\\
        & x^{2}+x
    \end{aligned}
\right
\end{equation}
```
    >`\{`用于输出大括号

## 表格
* 普通表格环境tabular
```
\begin{tabular}{|l|c|r|}
    \hline
    指标1 & 指标2 & 指标3 \\
    \hline
    居左 & 居中 & 居右
    \hline
\end{tabular}
```

* 三线表的制作(需要booktabs宏包)
```
\begin{table}
\centering
    \caption{题目}
    \begin{tabular}{cccc}
        \toprule
        &指标1 & 指标2 & 指标3 \\
        \midrule
        方案一 & 1 & 0.5 & 100 \\
        方案二 & 2 & 0.6 & 200 \\
        \bottomrule
    \end{tabular}
\end{table}
```

## 图片
```
\graphicspath{{figures/},{pics/}}
```
>将图片与figures文件夹建立关联，即.tex文件与figures文件在在同一目录下，且此文档中用到的图片均来自figures这个文件夹

figure环境
```
\begin{figure}[H]
    \centering
    \includegraphics[width=8cm,height=12cm]{name.png}
    \caption{标题}
\end{figure}
```

>`[H]`固定图片位置

## 命令lable及引用
1. lable
```
lable{#1: #2}
```
    >`#1`表示类型，包括 `eq` 公式，`tab` 表格，`fig` 图片
`#2`表示名字

    ```
\begin{equation}
    F=ma
    \lable{eq:Niudun}
\end{equation}
```

2. ref
`\ref{eq:Niudun}`
```
...
由公式(\ref{eq:Niudun})我们可知
...
```

## 符号`&`与`\\`
* 符号`&`表示对齐
* 符号`\\`表示换行
* 特殊符号输出使用`\verb`