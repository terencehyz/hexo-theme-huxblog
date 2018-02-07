---
layout:     post
title:      "JavaScript 数据类型"
date:       2017-02-04 22:00:00
author:     "Terence Han"
header-img: "https://ws1.sinaimg.cn/large/77ce63b1ly1fceu1ztdvrj21gs0o674n"
comments: true
tags:
    - JavaScript
---
## JavaScript 数据类型

JavaScript是一个弱类型语言，具有基本类型和引用类型。对于JavaScript来说，万物皆对象（对象是拥有属性和方法的数据，属性是与对象相关的值，方法是能够在对象上的操作）

### 基本类型和引用类型

 - 基本类型：Undefined/Null/Boolean/Number/String/Symbol
 - 引用类型：Object/Array/Function/Date/RegExp...

### 类型的判断

`typeof`和`instanceof`这两个操作可以用来判断类型，但是有时会出现问题。
基于JavaScript中的万物皆对象，

```JavaScript
/* 检测对象类型
 * @param: obj {JavaScript Object}
 * @param: type {String} 以大写开头的 JS 类型名
 * @return: {Boolean}
*/
function is(obj, type)  {  
  return Object.prototype.toString.call(obj).slice(8, -1) === type;
}
```

我们可以利用`is`这个函数来判断数据类型

```JavaScript
is('sofish', 'String') // true  
is(null, 'Null') // true  
is(new Set(), 'Set') // true
```

### 类型转换

JavaScript中的数据类型是可以改变的，如：

```JavaScript
1 + '2' // '12'  
1 + (+'2') // 3  
1 - '2' // -1  
```

在JS中，`+`具有双重角色，在上面的第二个例子当中，`String`前面的`+`把其强制转换为`Number`。对于JS的类型转化通常理解`+`具有双重角色即可