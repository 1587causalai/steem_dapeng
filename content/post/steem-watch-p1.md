---
title: "谷哥点名第 1 期“精彩瞬间”回顾（大鹏观察 Steem's Watch P1）"
author: dapeng
date: "2017-08-22 22:10:45"
slug: steem-watch-p1
categories: [cn]
tags: 
  - cn
  - blog
  - cn-blog
  - steemit
  - steem
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/steem-watch-p1), [cnsteem](https://cnsteem.com/cn/@dapeng/steem-watch-p1), [chainbb](https://chainbb.com/cn/@dapeng/steem-watch-p1), [busy](https://busy.org/cn/@dapeng/steem-watch-p1), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/steem-watch-p1.md)

不久前，为了玩得开心，我把"谷哥点名"第一期活动参与的帖子[整理成了一本电子书](https://steemit.com/cn/@dapeng/6wpnvk)。后来，在做“[大鹏观察](https://steemit.com/cn/@dapeng/steem-id-report-1-justyy-1) ”活动时，觉得与其单纯整理电子书，还不如用类似的方法对参赛帖子进行一些数据分析和挖掘，也许更有指导意义。于是，就有了“大鹏观察”之“谷哥点名”。本文是第一期，对谷哥点名第一期进行回顾。第二期很快就可以出台了，争取赶上谷哥点名的进度。欢迎大家提意见反馈。


用的数据来源是 steemdata.com，数据获取、分析、报告编写全程使用人见人爱的 R 语言。仅供参考，如果有数字与官方不符，请以官方数字为准。


## 大鹏观察： 谷哥点名第一期回顾


### 参赛基本信息


-   主题：精彩瞬间

-   日期：2017-08-02 -- 2017-08-09

-   发起：[关于“谷哥点名”游戏的初步设想](https://steemit.com/cn/@jubi/42wvdr)

-   颁奖：[第一期“谷哥点名”活动结束 & 第二期开始！](https://steemit.com/cn/@jubi/4tsdsb-and)

-   参赛作品列表：见文末。


### 帖中之最


本期活动参赛作品共 26 篇。获奖作品的介绍已经在本文开头给出了链接，是按 google 搜索结果排名的，不再赘述。我们也可以用其他方式排名，来看看参赛作品里几个第一名。


**字符最多**


-   [長毛家的毛寶貝\#4 : 二毛帶給我生活中無數的精彩瞬间 Pets in our family\#4: The countless wonderful moments Er-Mao brings to me](https://steemit.com/@catwomanteresa/4)，含 4833 个字符。


**插图最多**


-   [長毛家的毛寶貝\#4 : 二毛帶給我生活中無數的精彩瞬间 Pets in our family\#4: The countless wonderful moments Er-Mao brings to me](https://steemit.com/@catwomanteresa/4)，含 13 张图片。


**修改间隔最长.**


-   [记录那些值得回忆的精彩瞬间](https://steemit.com/@justyy/5hgpar)，发布 93.1 小时即 3.9 天之后，作者做了最后一次修改。


**得赞最多**


-   [我的三个精彩瞬间/Three of My Wonderful Moments](https://steemit.com/@mrpointp/three-of-my-wonderful-moments)，得到 124 个赞。


**赚钱最多**


-   [精彩瞬间-施比受更有福](https://steemit.com/@angelababy/7vearl)，收入为 48 美元。


**帖子正文里出现最多的关键词**


下面是所有帖子里出现的字符长度超过2个、出现次数超过10次的中文关键词词云图。字符越大，在全部帖子里重复出现的次数就越多。当然，我们去掉了“精彩瞬间”。


![unnamed-chunk-7-1.png](https://steemitimages.com/DQmdD6LnAyqQaafMqZmj3aR7QvDT1WMKeU7mvQsq5hqfDBt/unnamed-chunk-7-1.png)


### 参赛选手


下图是参赛选手的注册id序号分布图。全网目前共有 313128 个 ID。参赛选手中排在最前面的是第 18783 个 ID，最后面的是 第 289368 个 ID。猜猜他们都是谁？


![unnamed-chunk-8-1.png](https://steemitimages.com/DQmP3Q2v8wMuF87ykkm5T2RBmyKWT5yFrVS6PXMNAu925YY/unnamed-chunk-8-1.png)


下图是参赛选手的注册日期分布图。大部分参赛者都是 2017 年 5 月后注册的新朋友，尤其是 2017 年 7月注册的居多。


![unnamed-chunk-9-1.png](https://steemitimages.com/DQmTzghBuNYqSFgA8hmoxkKGzjxXz69WpqoUVwHhmcufrsN/unnamed-chunk-9-1.png)


### 发帖


活动期间，每天累计发帖总数：


![unnamed-chunk-10-1.png](https://steemitimages.com/DQmRY4GR1MBjA9X5dEBFN3HsErJn6pLmNjeiUpVsnXBCB1E/unnamed-chunk-10-1.png)


下图是个特殊的时钟，一圈是24小时，显示了一天24小时里发帖的频次，面积越大的时段，发帖数就越多。红线显示的是频次分布：每两条相邻红线之间的???子数，占全部帖子数的 25%。哪两条红线最接近，哪两条红线之间就是发帖高峰时段。


可以发现，在标准时间 2 点到 10 点发帖的人最多。大家猜猜这是为什么？我觉得这说明参赛者里位于欧洲的比较少。


![unnamed-chunk-11-1.png](https://steemitimages.com/DQmY6APo4VqwY7jPCbrV52XuGmNysA3kYvcYrtMSgeXhxTv/unnamed-chunk-11-1.png)


本活动是在 'cn' 板块发起的，参加活动的帖子自然都贴上了该标签以及子区标签。我们看看除此之外，大家还使用了那些标签以及使用频率。


![unnamed-chunk-12-1.png](https://steemitimages.com/DQmf2E9BhNokFAjGu16xnwFAjUskmGC4w34dpkSaZ8MDzi8/unnamed-chunk-12-1.png)


最显眼的标签是什么？我觉得是 jubi， 你觉得呢？


### 收入


最后我们来谈钱。下图显示的是单篇帖子收入的分布。横坐标是美元，阴影面积越大，对应美元的帖子数量越多。 参与活动的 26 篇帖子，总收入为 112.11 SBD， 单帖收入最高为47.87 SBD，平均每帖收入为4.31 SBD。


![unnamed-chunk-13-1.png](https://steemitimages.com/DQmcR4DG4n2axeLDksnyqRt1oHuRmnW1YqN66cX1Spwwh8R/unnamed-chunk-13-1.png)


下图是各篇帖子获得的投票（点赞）数。 累计得赞 1022 个，单帖得到的点赞数最高为 124 个，平均每帖得赞 39.3 个。


![unnamed-chunk-14-1.png](https://steemitimages.com/DQmbecakvFPpySzdkufYpGqSGqcsYUBZNDmhX63G3txBq87/unnamed-chunk-14-1.png)


为本次活动能够投票次数最多的前三位是 @jubi, @abit, @lordp。下面是投票次数超过 10 次的 ID 词云图。


![unnamed-chunk-15-1.png](https://steemitimages.com/DQmcEqJVEUUN79TcGBVmyajhq1Bpc1DZUkV2CwcWpW9TjhA/unnamed-chunk-15-1.png)


为本次活动点赞收入贡献最多的前三位伯乐是 @abit, @tumutanzi, @trafalgar。他们一共贡献了全部收入的 85%。感谢他们的支持！


------------------------------------------------------------------------


感谢关注“大鹏观察”。欢迎参加下一期的活动，也欢迎提出宝贵意见。谢谢。


### 附录：参赛作品列表


| created             | author            | title                                    |
| :------------------ | :---------------- | :--------------------------------------- |
| 2017-08-02 04:06:24 | @fundurian        | [谈谈精彩瞬间](https://steemit/com/@fundurian/hdv45) |
| 2017-08-02 05:20:18 | @mrspointm        | [The wonderful moment from a foodie / 来自一枚吃货的精彩瞬间](https://steemit/com/@mrspointm/the-wonderful-moment-from-foodie) |
| 2017-08-02 06:16:15 | @mrpointp         | [我的三个精彩瞬间/Three of My Wonderful Moments](https://steemit/com/@mrpointp/three-of-my-wonderful-moments) |
| 2017-08-02 07:23:12 | @coldhair         | [热爱生活，每一刻都是精彩瞬间](https://steemit/com/@coldhair/6vdmca) |
| 2017-08-02 09:19:00 | @larus            | [游戏X生活中的那些精彩瞬间，值得记录！](https://steemit/com/@larus/x) |
| 2017-08-02 12:07:36 | @dixonloveart     | [回首过去，难忘的3个精彩瞬间 Three Moments worth remembered in the last 2 years](https://steemit/com/@dixonloveart/3-three-moments-worth-remembered-in-the-last-2-years) |
| 2017-08-02 22:42:51 | @justyy           | [记录那些值得回忆的精彩瞬间](https://steemit/com/@justyy/5hgpar) |
| 2017-08-03 01:55:51 | @htliao           | [我的精彩瞬间](https://steemit/com/@htliao/3i973e) |
| 2017-08-03 02:23:12 | @syh7758520       | [在steemit的几个精彩瞬间](https://steemit/com/@syh7758520/34w14j-steemit) |
| 2017-08-03 12:35:45 | @kitcat           | [我的精彩瞬间 －苦尽甘来的哲理](https://steemit/com/@kitcat/5sngfq) |
| 2017-08-03 14:18:57 | @catwomanteresa   | [長毛家的毛寶貝\#4 : 二毛帶給我生活中無數的精彩瞬间 Pets in our family\#4: The countless wonderful moments Er-Mao brings to me](https://steemit/com/@catwomanteresa/4) |
| 2017-08-03 15:39:00 | @kenchung         | [我們的精彩瞬间](https://steemit/com/@kenchung/6acthe) |
| 2017-08-03 15:57:48 | @tvb              | [藏头诗：七绝-精彩瞬间（中华新韵）Acrostic Poem of Wonderful Moment](https://steemit/com/@tvb/acrostic-poem-of-wonderful-moment) |
| 2017-08-04 05:59:51 | @superhardness    | [Wonderful and ordinary moment--精彩瞬间与平凡同行](https://steemit/com/@superhardness/wonderful-and-ordinary-moment) |
| 2017-08-05 09:11:30 | @chaofanjun       | [我的生活哪有精彩瞬间？](https://steemit/com/@chaofanjun/5oy7zz) |
| 2017-08-06 18:54:42 | @tumutanzi        | [精彩瞬间带来美好回忆——中年大叔的人生故事](https://steemit/com/@tumutanzi/7enuof) |
| 2017-08-07 04:12:45 | @towardsthesun    | [My first steemit post - a beautiful moment // 精彩瞬间让我们更勇敢](https://steemit/com/@towardsthesun/my-first-steemit-post-a-beautiful-moment) |
| 2017-08-07 05:01:21 | @herlife          | [Wonderful Moments知足常乐，生活处处是精彩瞬间](https://steemit/com/@herlife/wonderful-moments) |
| 2017-08-07 07:46:36 | @blacktranquility | [骑行路上的精彩瞬间~水管](https://steemit/com/@blacktranquility/mbtqr) |
| 2017-08-07 08:31:18 | @dapeng           | [与周华健同台演出 \[视频 精彩瞬间\]](https://steemit/com/@dapeng/2wot2j) |
| 2017-08-07 12:53:12 | @zhijun           | [生命至今的三个精彩瞬间](https://steemit/com/@zhijun/5spugd) |
| 2017-08-07 16:46:18 | @timknip          | [新witness节点上线了，fuli 精彩瞬间](https://steemit/com/@timknip/witness-fuli) |
| 2017-08-07 21:00:36 | @joythewanderer   | [我难忘的几个精彩瞬间 Memorable Moments in my Life](https://steemit/com/@joythewanderer/memorable-moments-in-my-life) |
| 2017-08-08 00:46:36 | @guyverckw        | [人生中最「精彩瞬间」的事件！](https://steemit/com/@guyverckw/4jwkyd) |
| 2017-08-08 01:40:15 | @victorier        | [谈一谈我与精彩瞬间](https://steemit/com/@victorier/3to5b4) |
| 2017-08-08 15:27:12 | @angelababy       | [精彩瞬间-施比受更有福](https://steemit/com/@angelababy/7vearl) |


Tags: #blog #cn-blog #steemit #steem
