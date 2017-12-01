---
title: "另类方式秀恩爱"
author: dapeng
date: "2017-11-30 16:18:33"
slug: 5ukx1b
categories: [cn]
tags: 
  - cn
  - science
  - mathematics
  - blog
  - howto
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/5ukx1b), [cnsteem](https://cnsteem.com/cn/@dapeng/5ukx1b), [busy](https://busy.org/cn/@dapeng/5ukx1b), [chainbb](https://chainbb.com/cn/@dapeng/5ukx1b), [steemdb](https://steemdb.com/cn/@dapeng/5ukx1b), [steemd](https://steemd.com/cn/@dapeng/5ukx1b), [busy](https://busy.org/cn/@dapeng/5ukx1b), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_dapeng/master/content/post/5ukx1b.md)

秀恩爱，方式不一而足，不一定要贴照片。比如，有人选择去面馆吃面，有人则要直播吃辣椒。我也凑个热闹。我秀恩爱的方式是——

![](https://cdn.pixabay.com/photo/2015/10/30/12/24/questions-1014060_960_720.jpg)

## 背景

媳妇甩给我一堆 Matlab 代码：去，给我转成 R 语言。

这是个关于大气化学的常微分方程。Matlab 代码已经解出来了。但是，媳妇考虑到日后维护和拓展的需要，就想换成 R。

娶个女博士做老婆是怎样一种体验？挪，就是这种体验。

好在难不倒我。作为资深 R 语言爱好者，三下五除二，我将它转成了 R 代码。

解是解出来了，但是，得到的解差别很大。

Matlab 提供了一系列解常微分方程的函数，例如 ode15s, ode23s, ode23t, ode23tb 等。我手头代码里用的是 ode23tb。

R 语言的 deSolve 包提供了解常微分方程的函数 `ode()`，其中可用的参数 method 可以是以下取值：

```
method = c("lsoda", "lsode", "lsodes", "lsodar", "vode", "daspk",
           "euler", "rk4", "ode23", "ode45", "radau", 
           "bdf", "bdf_d", "adams", "impAdams", "impAdams_d", "iteration")
```
里面不包括 ode23tb 方法。我写的 R 代码里用了默认的 lsoda 方法，导致得到的解跟 Matlab不同。


## 我做过的测试

我找了个简单的常微分方程，来自 [Matlab 在线帮助](https://cn.mathworks.com/help/matlab/ref/ode23tb.html)：

d*y*/d*t* = - 10*t*

我分别用 Matlab 和 R 对它求解。

Matlab 解法：

```
tspan = [0 2];
y0 = 1;
[t,y] = ode23tb(@(t,y) -10*t, tspan, y0);
```

R 语言解法：

```
tspan = seq(0, 2, 0.2)
y0 = 1
testf <- function(t, y, p){
  with(as.list(c(y, p)), {
    dydt = -a*t
    list(dydt)
  })
}
p <- list(a = 10)
zz <- deSolve::ode(y = y0, times = tspan, func = testf, parms = p)
```

二者得到的结果是不同的。ode() 未指定 method，默认用的是 lsoda。

我尝试了把二者都改为 ode23 方法。即把 Matlab 代码最后一行改为：

```
[t,y] = ode23(@(t,y) -10*t, tspan, y0);
```

并把 R 代码最后一行改为：

```
zz <- deSolve::ode(y = y0, times = tspan, func = testf, parms = p, method = 'ode23')
```

二者结算的结果就完全一致了。

但是，我手头要改的大气化学常微分方程，可能是因为太复杂，如果用 ode23 方法的话，无论 matlab 还是 R，计算时间都太长，花了12小时都没算完。


## 我的提问

Matlab 的 ode23tb 函数，在 R 语言里该如何实现？或者反过来，R 语言 deSolve 包 `ode()` 里的 "lsoda" 方法，如何在 Matlab 里实现？

我知道这个问题我不该问，但是我实在黔驴技穷了，发到这里碰碰运气，看有没有高人指点一下。这个事儿已经连续折磨我两天了，头发掉了一大把。

你说说，这算不算秀恩爱？
