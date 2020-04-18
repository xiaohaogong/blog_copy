---
title: Front-end Tip.
date: '2019-10-20'
metaDesc: "Some small knowledge of front-end development,I don't know what to write,Just share some simple getting started."
socialImage: true
tags:
  - javascript
---

- js 的数据类型有哪些?

  简单数据类型: `String` `Number` `Boolean` `Null` `Undefind`  
   复杂数据类型:`Object`  
   所有对象派生自`Object`,`Undefind`类型只有一个值`undefind`,`Null`类型只有一个值`null`
  未定义或者定义未赋值的变量,对其进行`typeof`类型获取的时候,得到`undefind`
  `undefind`和`null`的异同
  `undefind`值派生自`null`,所以`null==undefind`为 true

  `null` 是空指针,我理解为空对象指针,`undefind`连指针也没有,所以`null==undefind`为 false

  ```javascript
  Number(null); //结果为0
  Number(undefind); //NaN
  ```

  - Json 和 javascript 对象的异同,如何进行转换？

Json 是一种数据传输格式,是以字符串的形式。

Json 对象是 javascript 对象的子集,Json 对象没有方法,只有属性键值对

Json 字符串转换为 Json 对象

```javascript
var str = '{"name":"koi"}';
eval("(" + str + ")"); //eval方法的弊端是：1.安全性问题。2.代码如果出错会导致程序崩溃并退出。3.全局变量污染        。
JSON.parse(str); //安全的做法
```

Javascript 对象转为 Json 字符串

```javascript
JSON.stringify(o);
```

什么是闭包?
内部函数访问到外部变量,反之外部函数无法获取到内部函数的变量,就是一个闭包

https://developer.mozilla.org/en-US/docs/Glossary/JavaScript









