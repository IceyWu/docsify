#### 为多个变量赋值

```js

// 常规写法 
let a, b, c; 
a = 5; 
b = 8; 
c = 12;

// 简写
let [a, b, c] = [5, 8, 12];

```

#### 多条件检查

```js

// 常规写法
if (value === 1 || value === 'one' || value === 2 || value === 'two') { 
     // 执行一些代码
} 

// 简写1
if ([1, 'one', 2, 'two'].indexOf(value) >= 0) { 
    // 执行一些代码 
}
// 简写2
if ([1, 'one', 2, 'two'].includes(value)) { 
    // 执行一些代码 
}

```

#### 字符串（String）转为数字（Number）

* 有一些内置方法，如 parseInt 和 parseFloat ，可以将字符串转换为数字。我们也可以通过简单地在字符串值前面提供一个一元运算符 + 来实现。

```js
// 常规写法
let total = parseInt('453'); 
let average = parseFloat('42.6'); 

// 简写
let total = +'453'; 
let average = +'42.6';

```



#### 合并数组

```js
let arr1 = [20, 30]; 

// 常规写法
let arr2 = arr1.concat([60, 80]); 
// [20, 30, 60, 80] 

// 简写
let arr2 = [...arr1, 60, 80]; 
// [20, 30, 60, 80]
```