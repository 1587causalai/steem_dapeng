---
title: "Recent Three Months on Steem - 最近三个月"
author: dapeng
date: "2017-12-18 23:05:24"
slug: recent-three-months-on-steem-or
categories: [cn]
tags: 
  - cn
  - steemit
  - news
  - cn-reader
  - stats
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/recent-three-months-on-steem-or), [cnsteem](https://cnsteem.com/cn/@dapeng/recent-three-months-on-steem-or), [busy](https://busy.org/cn/@dapeng/recent-three-months-on-steem-or), [chainbb](https://chainbb.com/cn/@dapeng/recent-three-months-on-steem-or), [steemdb](https://steemdb.com/cn/@dapeng/recent-three-months-on-steem-or), [steemd](https://steemd.com/cn/@dapeng/recent-three-months-on-steem-or), [busy](https://busy.org/cn/@dapeng/recent-three-months-on-steem-or), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_dapeng/master/content/post/recent-three-months-on-steem-or.md)

> A friend asked me about the recent trends in  ID sign-ups and posts on steem. I was also wondering if there is decrease in new sign-up. Remember [Ned undelegated his SP from some Chinese users](https://steemit.com/steemit/@dapeng/can-the-gossip-tell-us-why-ned-undelegated-sp-the-answer-is-no)? Did the undelegation have impact on CN community? Let's have a look at the data from steemsql.

最近这些天，闭关熬论文，至于 steem 上发生了什么，我是不知有汉，无论魏晋。好在还有朋友惦记，托我查看一下最近三个月 steem 的账号注册和活跃情况，尤其是华语区的情况。好吧，我也一直想看看自从临时大鲸们卸任后的变化：是不是新人越来越少了？是不是旧人越来越懒了？在 [Ned 收回代理给临时大鲸鱼的 SP](https://steemit.com/steemit/@dapeng/can-the-gossip-tell-us-why-ned-undelegated-sp-the-answer-is-no) 之后，华语区是否真的变冷了？——我感觉不是，因为我的机器人每天发布的[新人希望工程日报](https://steemit.com/@pzhao)显示，最近 CN 区的发帖数每天超过 300，比临时大鲸鱼活跃时期发帖更多。

下面的数据来自 steemsql 数据库，数据获取和统计用的是 R 语言。

### The entire site | 全网情况

为了描述方便，我们先下个定义：

- “活跃账号"，指的是必须在最近 90 天里发过至少一篇 blog 的账号。

- “新账号”，指的是到今天为止注册未满 90 天的账号。

首先，我们先看看 steet 上的账号总数，注册用户共有 502105 个。那么活跃账号是 91892 个，占账号总数的 18%。是的，在最近三个月里，全网 ID 每 5 个账号里只有一个发过帖子，另外 4 个基本、已经、死了。

下图显示了每天新注册的用户数量（蓝色）和其中活跃的数量（橘色）。最近 90 天内，共注册 129056 个新用户，平均每天 1434个。这些新 ID 里，发过帖子的有 48531 个，占全部新 ID 的 38% 。也就是说，每 5 个新 ID 里，有 2 个发过帖子。

>  There are 502105 IDs in total, 18% of which are active. The following image shows the daily new sign-ups (blue) and the active user number (orange) in the recent 90 days. 38% of the new IDs have posted.  *New IDs* means those whose steem age is younger than 90 days.

![unnamed-chunk-3-1.png](https://steemitimages.com/DQma6qouzK5Lk9Y7nw2WZM3bzRGrbP2KekiNvWTqsUhEmAj/unnamed-chunk-3-1.png)

下图显示了是全网每天的发帖总数（蓝色）和其中来自新账号的发帖数（橘色） 。

> The following image shows the daily post quantity (blue) and those from new IDs (orange).

![unnamed-chunk-5-1.png](https://steemitimages.com/DQmaMr2TepwNyaf1dcR3EuhNQdQ7E6JCW5enCjwbascz85v/unnamed-chunk-5-1.png)

CN category | CN 区情况
---------

下面，我们用类似的方法，看看 CN 区的情况。下图是每天来 CN 区发帖的用户数量（蓝色）和其中新用户的数量（橘色）。

> The following image shows how many IDs posted in CN category everyday (blue), and how many of them are new IDs (orange).

![unnamed-chunk-7-1.png](https://steemitimages.com/DQmfLNBdRUm5CymZhfTxgchFQrFLvqZeiDuFhFawuwo3Scw/unnamed-chunk-7-1.png)

下图显示了是 CN 区每天的发帖总数（蓝色）和其中来自新账号的发帖数（橘色） 。最近半个月呼呼猛涨，是出大事儿了吗？我一定在闭关时错过了什么……

> The following image shows the daily post quantity (blue) and those from new IDs (orange) in CN category.

![unnamed-chunk-9-1.png](https://steemitimages.com/DQmeck5JDm4KJMpwPYTgU8gQyvG76VWNNFZXUK1SbRqANeU/unnamed-chunk-9-1.png)

CN-READER Sub-category | CN-READER 子区情况
----------------

我们特别看看 cn-reader 子区的情况。下图是每??来 cn-reader 子区发帖的用户数量（蓝色）和其中新用户的数量（橘色）。

> The following image shows how many IDs posted in CN-READER category everyday (blue), and how many of them are new IDs (orange).

![unnamed-chunk-11-1.png](https://steemitimages.com/DQmfNE3qoK7mrxERZU2KFcCXcAGzMRjgCpaz9fTeq5g8xcw/unnamed-chunk-11-1.png)

下图显示了是 cn-reader 子区每天的发帖总数（蓝色）和其中来自新账号的发帖数（橘色） 。

> The following image shows the daily post quantity (blue) and those from new IDs (orange) in CN-READER sub-category.

![unnamed-chunk-13-1.png](https://steemitimages.com/DQmWPwjtcnmzsVdD4bbwPYZHPiECkZMTvptzPW8GEQCpYFC/unnamed-chunk-13-1.png)

> Do you remember when @ned undelegated his SP from the Chinese users?
>
> It was Oct. 24, 2017, when we said *Winter is coming*. 
>
> After only one month or so, the ice is gone.
>
> Keep moving on and never give up.

那么大家还记得 Ned 是哪天收回他的 SP 吗？

是 2017 年 10 月 24 日。

那天，华语区哀鸿遍野，仿佛世界末日。

而如今，才过去几天，华语区的活跃度早就冰雪消融，万物复苏了。

留得青山在，不愁没柴烧。不论什么情况下，都不要抛下老婆孩子跳楼。看得远一点，永远都不要绝望，永远。
