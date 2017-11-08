---
title: "致歉：新人“三个一”颁奖乌龙事件 Letter of Apology for Mistakes in the Award Ceremony"
author: dapeng
date: "2017-10-14 21:37:24"
slug: letter-of-apology-for-mistakes-in-the-award-ceremony
categories: [cn]
tags: 
  - cn
  - cn-reader
  - cn-31
  - cn-contest
  - contest
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/letter-of-apology-for-mistakes-in-the-award-ceremony), [cnsteem](https://cnsteem.com/cn/@dapeng/letter-of-apology-for-mistakes-in-the-award-ceremony), [chainbb](https://chainbb.com/cn/@dapeng/letter-of-apology-for-mistakes-in-the-award-ceremony), [busy](https://busy.org/cn/@dapeng/letter-of-apology-for-mistakes-in-the-award-ceremony), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/letter-of-apology-for-mistakes-in-the-award-ceremony.md)

2017 年奥斯卡颁奖典礼上，颁奖嘉宾把最佳影片奖颁给了 *La La Land*。当该影片的演职人员激动的捧过小金人向支持他们的亲朋好友一一道谢时，却被告之，奖发错啦！真正的获奖影片是 *Moonlight*。


真糗。我想。这要是我，那恨不得找个地缝钻进去。


哪知道，几个月之后，这一幕在我身上上演：今天早上的新人三个一活动颁奖典礼，我也把奖发！错！了！


![](https://c1.staticflickr.com/6/5086/5299579966_846d4cb9ea_b.jpg)


Image credit: c1.staticflickr.com


今天比较忙，一早匆匆发了帖，就出去遛娃了。期间看了一下 steemit 上的回复，有朋友提醒我，说可能我把文章的评论人数算错了。我大吃一惊，心急如焚，但是没办法，带娃的时候不可能去查数据。所以在此我奉劝那些单身的或者还没生娃的朋友：珍惜你们的自由时光吧，这是你们玩 steemit 的好时候。等一有了娃，就身不由己咯。


带了一天娃，累个半死，终于都伺候睡了，我就核查数据。我用的是 steemsql 数据库。再三检查，我发现一个非常奇怪的现象：steemit 上看到的某篇文章的回复，跟数据库里查询的结果有不同。


比如『[回望我的25岁|“三个一”活动](https://steemit.com/cn/@acactus1013/25) 』这篇文章，steemit 上显示的回复人数，扳着指头数了数是 15 个（包括作者本人）。但是，steemsql 数据库里，搜 root_title 为**回望我的25岁|“三个一”活动**的回复，人数只有 11 个。有 4 个人，例如 @veronicazhu 的回复，没有列在里面。


这里说说 root_title 是什么。每条回复信息，在 steemsql 数据库里都有对应的发布时间、作者、链接等信息。怎么判断一条回复属于哪个帖子呢？有个 root_title 字段，显示的就是帖子的标题。理论上，只要筛选出**回望我的25岁|“三个一”活动**标题的回复，就行了。那为什么漏了？


我还以为时间范围弄错了，反复检查无误。这就奇怪了。


于是我搜漏掉的 @veronicazhu 发布的所有回复，逐条检查，终于发现，有一条回复的帖子标题是**回望我的25岁**！不包含**三个一活动**这几个字！难怪没搜到！


于是，我把**回望我的25岁|“三个一”活动**和**回望我的25岁**两个标题所有的回复都找出来，发现这样就齐全了！


![31error.jpg](https://steemitimages.com/DQmYM6mQgCwkZ2XMbF6huZ8MsjKB3pWv1T9pr83st42ZbGu/31error.jpg)


对此，我的推测是，可能作者 @acactus1013 在发布文章后修改过标题，于是文章的回复就被分到了不同的标题下面。而我原以为一篇文章的 root_title 字段是不会更改的——事实上，颁奖前我抽查了两三篇文章，不幸的是这两三篇的标题恰恰没改过——于是就导致了颁奖的乌龙事件！


steemsql 没有明确的使用说明书，很多东西靠猜。经过这个事件，我发现，判断一条回复属于哪篇文章，不能用 root_title ，而需要用 root_comment，这是个整数，跟每篇文章唯一对应，不会更改。


下面是经过修正的获奖者名单：


| 奖项   | 作者           | 标题                                       | 评论人数 |    收益 |    赞 |
| :--- | :----------- | :--------------------------------------- | ---: | ----: | ---: |
| 金奖   | @acactus1013 | [回望我的25岁-“三个一”活动](https://steemit.com/cn/@acactus1013/25) |   15 | 20.68 |   32 |
| 银奖   | @xiaoshancun | [地瓜花与母亲的渴望](https://steemit.com/cn/@xiaoshancun/4ykg3k) |   14 | 18.80 |   31 |
| 放弃   | @xiaoshancun | [错过风景，???能错过一个你](https://steemit.com/cn/@xiaoshancun/7tlug7) |   13 | 19.74 |   44 |
| 铜奖   | @victory622  | [望 - steem 华语区新人"三个一"活动 - 我唱了首名字叫做《望》的歌](https://steemit.com/cn/@victory622/steem) |   13 | 19.21 |   62 |


以上名单和全部参赛作品的统计数据，已经在『[新人“三个一”活动第 1 期颁奖典礼](https://steemit.com/cn/@dapeng/1-or-awards-ceremony-for-the-welcome-prize-new-steemians)』一文中做了更正。


乌龙事件当然不能怪作者修改标题。这完全是我一个人的疏忽导致的。在此，我向所有参加或关心本活动的朋友们郑重道歉，尤其是向前三名获奖者道歉。已经错发出去的奖金不再收回，漏发的奖金已经由我个人出资补发。感谢提醒我的朋友，请大家继续监督我的工作，继续关注新人”三个一”的第二期活动！谢谢！





Tags: #cn-reader #cn-31 #cn-contest #contest


![大鹏](https://steemitimages.com/DQmeYUwQ7Juorgd79o6D5E34BnUYxwfmLxYH4cApgPRhRf6/end2.jpg)
