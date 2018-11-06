# 第11课：操作符（Operators）

先看看Python有哪些常用操作符：
```
+       -       *       **      /       //      %      @
<<      >>      &       |       ^       ~
<       >       <=      >=      ==      !=
```

### 算术操作符
+, -, *, / , %, // , **, _ 分别为加、减、乘、浮点除、取余数（返回除法的余数）、整数除（返回商的整数部分）、幂运算（x的y次幂）、上个表达式结果的值。
```
>>> a = 2
>>> b = 6
>>> a + b
8
>>> a - b
-4
>>> a * b
12
>>> a/b
0.3333333333333333
>>> a % b
2
>>> b % a
0
>>> a ** b
64
>>> a // b
0
>>> b // a
3
>>> _
3
```

### 比较操作符
==, !=, <, >=, <= 分别为相等、不等于、大于、小于、大于等于、小于等于。
```
>>> (a == b)
False
>>> (a != b)
True
>>> (a > b)
False
>>> (a < b)
True
>>> (a >= b)
False
>>> (a <= b)
True
```

### 位操作符
按位运算符是把数字看作二进制来进行计算，数字加上前缀 '0b' 表示是二进制数字。

&, |, ^, ~, << , >> 分别为按位与、或、异或、取反、左移、右移。

自己用2和4的二进制数做按位运算，并理解其结果。
```
>>> bin(2);bin(4)
'0b10'
'0b100'
>>> (0b10 & 0b100)
0
>>> (0b10 | 0b100)
6
>>> bin(6)
'0b110'
>>> (0b10 ^ 0b100)
6
>>> (0b10 << 2)
8
>>> bin(8)
'0b1000'
>>> (0b10 >> 2)
0
>>> bin(0)
'0b0'
>>>
```

### 逻辑操作符
and, or, not 分别为与、或、非。
```
>>> (a and b)
10
>>> (a or b)
21
>>> not(a and b)
False
```

### 成员操作符
in, not in 分别为是成员、不是成员。
```
>>> a = 1; b = 2
>>> list = [1, 2, 3, 4, 5]
>>> (a in list)
True
>>> (c not in list)
True
>>> (b not in list)
False
```

### 身份运算符
is, is not 分别为同一对象、不是同一对象。
```
>>> a = 1; b = 2
>>> (a is b)
False
>>> (a is not b)
True
```

### 赋值操作符
把算术运算符和=组合起来使用。
```
>>> c = a + b
>>> c
8
>>> c += a
>>> c
10
>>> c -= a
>>> c
8
>>> c *= a
>>> c
16
>>> c /= a
>>> c
8.0
>>> c %= a
>>> c
0.0
>>> c **= a
>>> c
0.0
>>> c //= a
>>> c
0.0
```

### 运算符优先级
```
>>> a = 10; b = 6; c = 3; d = 0
>>> a = 10; b = 6; c = 3; d = 2
>>> ((a + b) * c) / d
24.0
>>> a * b ** c
2160
>>> a * (b ** c)
2160
```

配图来自Twitter

![配图11](https://wiki.huihoo.com/images/e/ef/Devopsgirls11.jpg)