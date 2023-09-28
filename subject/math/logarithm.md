---
title: 什么是对数？
date: 2023-09-28T14:47:45+08:00
updateDate: 2023-09-28T19:32:15+08:00
slug: subject/math/sequence/logarithm
image: 
categories:
  - 学科
tags:
  - 数学
  - 对数
draft: false
---
## 前言
比如现在来看一组幂运算（也叫求幂）：
- 2<sup>2</sup>，2的2次方，也就是2×2，结果是4。
- 2<sup>3</sup>，就是2×2×2，结果是8，其中2是底数，3是指数。

那假如只给出结果16，底数是2，2<sup>x</sup> = 16，求x也就是指数是多少？要怎么做？

猜得没错，这里就需要用到对数去解决。

## 概念
对数是求幂的逆运算，正如除法是乘法的逆运算，定义为$N = a^x (a > 0, a \neq 1)$，即a的x次方等于N。

记作 $x = log_aN$ ，也就是 $a^x = N$ 等同于$x = log_aN$

其中：
- a叫做底数。
- N叫做真数。
- x叫做以a为底N的对数。

> 以上面的例子为例，用对数的表示就是：$x = log_216$

- 当底数a=10的时候，叫做常用对数，可以缩写为：$lgN$
- 当底数a=无理数e的时候，叫做自然对数，缩写为：$lnN$

### 性质
1. 零和负数无对数。
2. 1的对数为0，$0 = log_a1$，也就是$a^0 = 1$
3. 底数和真数相同时，对数是1，$1 = log_aa$，也就是$a^1 = a$

### 练习
1、将下面指数式写成对数式：
- $5^4=625$
	- 答：$4 = log_5625$
- $2^{-6} = \frac{1}{64}$
	- 答：$-6 = log2\frac{1}{64}$

2、将下面对数式写成指数式：
- $log_\frac{1}{2}16 = -4$
	- 答：$\frac{1}{2}^{-4} = 16$
- $log_2128 = 7$
	- 答：$2^7 = 128$

## 运算
$$a^x = M, \quad a^y = N$$
$$a^x \times a^y = a^{x+y}$$
$$M \times N = a^{x+y}$$
$$log_a(M \times N) = x + y$$

### 运算法则
1、$log_aN = \frac{log_mN}{log_ma}$（a＞0，且a≠1，m＞0，且m≠1，N＞0）

又称换底公式，用m替换a，m可以是任意一个数。

以 $log_216$ 为例，将2替换成10，就是 $\frac{log_{10}16}{log_{10}2}$ ，用计算器算一算：
- $log_{10}16$的精确结果是：1.204119982655948。
- $log_{10}2$的精确结果是：0.3010299956639812。
- 相除以后的精确结果是：4.000000000000077，计算器取了近似值，所以答案是4，先取近似值再相除或者用精确结果相除再取近似值都可以，取决于计算时的选择。

2、$log_a(MN) = log_aM + log_aN$（a＞0，且a≠1，M、N＞0）

对数的乘法法则。

3、$log_a\frac{M}{N} = log_aM - log_aN$（a＞0，且a≠1，M、N＞0）

对数的除法法则。

4、$a^{log_aM} = M$（a＞0，且a≠1，M＞0）

5、$log_{a^{m}}b^{n} = \frac{n}{m}log_ab$（a、b＞0，且a、b≠1）

## 疑问
1、为什么定义中$a > 0, a\neq1$？
因为这些取值都是没有意义的，所以要限制，比如：
- 当a=0时，无论指数是多少，最终结果都是0。
- 当a=1时，无论指数是多少，最终结果都是1。
- 当a＜0时，即负数时，求幂的结果可能会有两种情况，要么是正数要么是负数，带来的多义性无法保证对数运算结果的唯一性，比如：
	- 指数为奇数时，求幂的结果是负数。
	- 指数为偶数时，求幂的结果是正数。

## 参考
1. [对数\_百度百科](https://baike.baidu.com/item/%E5%AF%B9%E6%95%B0)
2. [03.什么是对数\_\_哔哩哔哩\_bilibili](https://www.bilibili.com/video/BV1Li4y1M7St?p=3&vd_source=030e90a2464f7af11a177beceaf9bdc8)
3. [指数函数、对数函数、幂函数 -快速入门到完美精通\_哔哩哔哩\_bilibili](https://www.bilibili.com/video/BV1Dh411s7TT)
4. [（高一）对数（一）（对数的基本性质和性质）\_哔哩哔哩\_bilibili](https://www.bilibili.com/video/BV18F411h78H/?spm_id_from=333.788&vd_source=030e90a2464f7af11a177beceaf9bdc8)