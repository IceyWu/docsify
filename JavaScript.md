### 数组(Array)

#### 合并数组

```js
let arr1 = [20, 30]

// 常规写法
let arr2 = arr1.concat([60, 80])
// [20, 30, 60, 80]

// 简写
let arr2 = [...arr1, 60, 80]
// [20, 30, 60, 80]
```



### 对象(object)
#### 对象键值简写

- JavaScript简写技巧：对象的键和值相同时，可以只写一个

```js
let name = '张三',
	age = 19;
// 常规写法
let obj = { name: name, age:age };

// 简写
let obj = { name, age };
```




### 数字(Number)
#### 数字分隔符

- 这是比较新的语法，ES2021 提出来的，数字字面量可以用下划线分割，提高了大数字的可读性。

```js
// 旧语法
let number = 98234567

// 新语法
let number = 98_234_567
```
#### 数字（Number）转为字符串（String）


```js
const value = 12345;
// 常规写法
`${value}`;
JSON.stringify(value);
value.toString();
String(value);

// 简写
value + '';
```

### 字符串(String)
#### 字符串（String）转为数字（Number）
- 有一些内置方法，如 parseInt 和 parseFloat ，可以将字符串转换为数字。我们也可以通过简单地在字符串值前面提供一个一元运算符 + 来实现。

```js
// 常规写法
let total = parseInt('453')
let average = parseFloat('42.6')

// 简写
let total = +'453'
let average = +'42.6'
```
#### 字符串重复若干次
- Javascript简写技巧：使用 字符串.repect(次数)而不是for循环

```js
let str = ''; 
// 常规写法
for(let i = 0; i < 5; i ++) { 
  str += 'Hello '; 
} 

// 简写
str = 'Hello'.repeat(5);
```
#### 多行字符
- Javascript简写技巧：使用模板字符串代替字符串拼接和转义字符‘\n’的使用

```js
// 常规写法
const str1 = "Time flies.\n" + "Time is money.\n" + "Time tries all.";

// 简写
const str2 = 
`Time flies.
Time is money.
Time tries all.`
```


### 杂项
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
#### 为多个变量赋值

```js
// 常规写法
let a, b, c
a = 5
b = 8
c = 12

// 简写
let [a, b, c] = [5, 8, 12]
```
#### 断路运算符（&&）断路某些操作

- JavaScript简写技巧：断路运算符（&&）断路某些操作

```js
// 常规写法
if (state) {
	show();
}

// 简写
state && show();
```
#### 交换变量的值

- JavaScript简写技巧：交换变量的值

```js
let x = 'Hello', y = 55; 
// 常规写法
const temp = x; 
x = y; 
y = temp; 

// 简写
[x, y] = [y, x];
```
