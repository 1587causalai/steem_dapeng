---
title: "Looking for contributors to R mf package"
author: dapeng
date: "2017-12-06 08:27:48"
slug: 6dngsm-looking-for-contributors-to-r-mf-package
categories: [utopian-io]
tags: 
  - utopian-io
  - matlab
  - programming
---

原文链接: [steemit](https://steemit.com/utopian-io/@dapeng/6dngsm-looking-for-contributors-to-r-mf-package), [cnsteem](https://cnsteem.com/utopian-io/@dapeng/6dngsm-looking-for-contributors-to-r-mf-package), [busy](https://busy.org/utopian-io/@dapeng/6dngsm-looking-for-contributors-to-r-mf-package), [chainbb](https://chainbb.com/utopian-io/@dapeng/6dngsm-looking-for-contributors-to-r-mf-package), [steemdb](https://steemdb.com/utopian-io/@dapeng/6dngsm-looking-for-contributors-to-r-mf-package), [steemd](https://steemd.com/utopian-io/@dapeng/6dngsm-looking-for-contributors-to-r-mf-package), [busy](https://busy.org/utopian-io/@dapeng/6dngsm-looking-for-contributors-to-r-mf-package), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_dapeng/master/content/post/6dngsm-looking-for-contributors-to-r-mf-package.md)

This article was posted in a wrong category on utopian.io and somehow removed from utopian. Following the suggestion by mcfarhat, here I am resubmitting it.

## Background

'mf' packge is an R package I have been developing for meteorological models. Now I am looking for contributors to help me solve the following problem.

I have ordinary differential equations (ODEs) in atmospheric chemistry. I have a Matlab script, written by another guy, which can solve them. Now I have converted it into R script. However, the results are different.

In Matlab many functions are available to solve ODEs, including ode15s, ode23s, ode23t, ode23tb. My Matlab script uses ode23tb.

The deSolve package in R provides a function `ode()`, where many methods are available：

```
method = c("lsoda", "lsode", "lsodes", "lsodar", "vode", "daspk",
           "euler", "rk4", "ode23", "ode45", "radau", 
           "bdf", "bdf_d", "adams", "impAdams", "impAdams_d", "iteration")
```

However, ode23tb is not included.


## What I have tested

I tested a simple ODE from [Matlab online help](https://cn.mathworks.com/help/matlab/ref/ode23tb.html):

d*y*/d*t* = - 10*t*

The Matlab script:

```
tspan = [0 2];
y0 = 1;
[t,y] = ode23tb(@(t,y) -10*t, tspan, y0);
```

My R script

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

The results are different. In the R scirpt, `ode()` uses the default method 'lsoda'.

If I use ode23 method in both scripts, i.e. in the Matlab script:

```
[t,y] = ode23(@(t,y) -10*t, tspan, y0);
```

while in R script：

```
zz <- deSolve::ode(y = y0, times = tspan, func = testf, parms = p, method = 'ode23')
```

They give the same results.

However, the atmosphereic chemistry ODEs I have to solve are complicated. If I use ode23 method, the calculation is too slow in both Matlab and R. 12 hours has passed and the calculation is still going on.


## My Problem

How can I use Matlab ode23tb function in R? Or how can I use "lsoda" method in Matlab?

Only by using the same method can I compare the results from Matlab and R.

Your contribution will be much appreciated and acknowledged in the mf package.

## Link to the repo and Proof of work

https://github.com/pzhaonet/mf

It is listed in my project page on utopian.io.

<br /><hr/><em>Posted on <a href="https://utopian.io/utopian-io/@dapeng/6dngsm-looking-for-contributors-to-r-mf-package">Utopian.io -  Rewarding Open Source Contributors</a></em><hr/>
