---
title: "豪华版 Steemit CN 微信群名单"
author: dapeng
date: "2017-09-02 14:15:54"
slug: steemit-cn
categories: [cn]
tags: 
  - cn
  - cn-programming
  - steemit-stats
  - wechat
  - ranking
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/steemit-cn), [cnsteem](https://cnsteem.com/cn/@dapeng/steemit-cn), [chainbb](https://chainbb.com/cn/@dapeng/steemit-cn), [busy](https://busy.org/cn/@dapeng/steemit-cn), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/steemit-cn.md)

前两天， [@bullda](https://steemit.com/@bullda) 做了个["Steemit好友微信群"排行榜](https://steemit.com/cn/@bullda/steemit)，我俩[商量了一下](https://steemit.com/cn/@bullda/steemit#@bullda/re-tumutanzi-re-bullda-re-xiaozuo-re-bullda-steemit-20170831t095541324z)，打算过两天做个动态在线表格。还没等动手， @justyy 已经[做出来了](https://steemit.com/cn/@justyy/steemit-daily-wechat-group-ranking-steemit)，真是心有灵犀。做得非常好，而且业界良心地提供了 超级好用的API。可惜的是，跟我设想的样子不大相同。


今天，我把设想的样子做出来了，称为“豪华版微信群名单”。豪华在哪里？


1、可以输入一个 ID，给出该 ID 的声誉、权力等各项指标排位座次，以及邻座坐的是谁。看看谁坐在我旁边：


![steemr.jpg](https://steemitimages.com/DQmUJSE478ZdswdSMv4zzFvSpyN4bWnLSHZmS2yjr1vQigw/steemr.jpg)


2、可以给定一个名次范围，画出该范围内的名单词云图，谁越排在前面，谁的名字就越大。


![steemr2.jpg](https://steemitimages.com/DQmNfdRYpyH4Fv2yVjTQnpRrLuZXCJ5ZddH1217aX4uoTBF/steemr2.jpg)


3、除了同样给出了全部名单列表，并且点击每列标题就可以顺序逆序外，还可以过滤。来，我们搜索一下声望值超过 70、注册时间为 410多 天的名单：


![steemr3.jpg](https://steemitimages.com/DQmVR7HyaaAi16eJ32YbKTnzqRqHJKA7UZwZkspxvJ8Bp7Z/steemr3.jpg)


豪华是有代价的：页面载入有点慢，需要个几秒钟，就看你有没有耐心。追求速度的话还是移步访问本文开头介绍那二位的网页吧。


这个排名座次有没有让你联想到什么？我联想到了很多，于是给这个名单取名为：


**Steem 中国聚义厅**


这个在线名单，作为一个组建，纳入??我开发的 steemr 小工具。steemr已经被收入 [steemtools.com](http://steemtools.com/)的列表里，直接访问地址是: 


http://steemr.org


steemr 是我刚来 steemit时开始开发的（[简介](https://steemit.com/cn/@dapeng/steemr-a-web-based-tool-for-steemers-or-steemians-steemr)），后来有朋友反馈了一些问题，这次顺手解决了，包括：


- Follower Report 里查询的 ID 粉丝太多时出现的问题，例如查询 @tumutanzi ，原来总是重载，后来发现是原始数据某个粉丝的数据格式问题没有得到兼容，现在已解决。

- Follower Report 新增韦恩图。

- 原来的“哪个粉丝没有赞某篇帖子”功能意义不大，删掉。


欢迎大家测（调）试（戏）和反（点）馈（赞）。
