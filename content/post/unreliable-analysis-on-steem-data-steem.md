---
title: "Unreliable analysis on Steem data 不靠谱的 steem 数据分析"
author: dapeng
date: "2017-09-10 16:24:24"
slug: unreliable-analysis-on-steem-data-steem
categories: [cn]
tags: 
  - cn
  - cn-programming
  - r-language
  - steemdata
  - mongodb
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/unreliable-analysis-on-steem-data-steem), [cnsteem](https://cnsteem.com/cn/@dapeng/unreliable-analysis-on-steem-data-steem), [chainbb](https://chainbb.com/cn/@dapeng/unreliable-analysis-on-steem-data-steem), [busy](https://busy.org/cn/@dapeng/unreliable-analysis-on-steem-data-steem), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/unreliable-analysis-on-steem-data-steem.md)

> First of all, I would like to thank @furion so much for providing [steemdata](https://steemdata.com/), and @arcange for [steemsql](http://steemsql.com/). Both have been helping me learn a lot about blockchain, and earn my first bucket of gold on Steem via "Steem's Watch" reports.


首先，我要深深感谢 @furion 提供了 [steemdata](https://steemdata.com/) 这个数据平台，感谢 @arcange 提供了 [steemsql](http://steemsql.com/)。二者极大地帮助我理解区块链，并让我通过“大鹏观察”系列报告赚到了我在steem上的第一桶金。


> I started my data analysis with steemdata and produces several reports. Many Steemians like them. However, I have found some strange problems recently.


我是从 steemdata 开始进行数据分析的，写了不少数据报告，幸运地得到了很多朋友的喜爱。然而，最近，我发现了一些奇怪问题。


> In the [account report of @hannahwu](https://steemit.com/cn/@dapeng/steem-hannahwu) I wrote two days ago, data from steemdata showed that @hannahwu had 227 followers and 165 followings.


两天前，我写了一份[ @hannahwu 的用户数据报告](https://steemit.com/cn/@dapeng/steem-hannahwu) 。来自 steemdata 的数据显示， @hannahwu 有 227 个粉丝，而她粉了 165 个账号。


![steemdataproblem2.jpg](https://steemitimages.com/DQmfThhbvG1hN6Y1SiiiWXfJYLbGwwVCJMADExzAjn9dxBj/steemdataproblem2.jpg)


> However, the profile of @hannahwu on Steemit showed 419 followers and 218  following. Now two days has passed, the data from steemdata are still the same. 


然而，她的 Steemit 主页却显示 419 个粉丝，粉了 218 个账号。现在，我写的数据报告已经发布了两天，我看了一下， steemdata 的这两项数据仍然没变。


![steemdataproblem2-1.jpg](https://steemitimages.com/DQmXxF7SukEoaTTYLJnMq9idc84KTYaPcA5GPJJxasK9gMu/steemdataproblem2-1.jpg)


> Another example is the account @ochedgreat, who has posted multiple posts recently. However, this account cannot be found in the Collection  of Accounts in steemdata, although @ochedgreat's posts are listed in the Collection of Posts. Does it mean that Accounts Collection is not compatible with the Posts Collection in steemdata?


另一个例子是账号 @ochedgreat，最近发布了多篇帖子。然而，在 steemdata  数据库的 Accounts 里却找不到这个账号。奇怪的是，@ochedgreat 的帖子却可以在 steemdata 的 Posts 里找到。这是不是说明，Accounts 和 Posts 两者并未同步？


![steemdataproblem1.jpg](https://steemitimages.com/DQmZZzsYYJrYknBNhAUtLtn5jf2PS4MeP9TdVWKftRYqSRG/steemdataproblem1.jpg)


> If you search ochedgreat on steemsql, you could find the account information. This account was created three days ago. Maybe it was too soon for steemdata to sync? 


如果在 steemsql 里查找ochedgreat，是能够找到账号信息的。该账号创建于三天前。是不是因为太新，还没被 steemdata 收录? 


![steemdataproblem1-1.jpg](https://steemitimages.com/DQmNmxbkbS1QSD7wsCSMe2iDrmyYXJNjJCocJmDPFRJtjDY/steemdataproblem1-1.jpg)


> I cannot find any hint on the official website of steemdata about the delay time of data synchronization. In [a post by @oflyhigh](https://steemit.com/cn/@oflyhigh/steemdata), it was mentioned that data are synchronized from the blockchain to steemdata in real time, which confused me even more.  Thus, I searched for the account created most lately.  The latest account in steemdata was @asn191, created on 2017-09-10 07:54:06 UTC. 


在 steemdata 的官网上，我没有找到关于数据更新时间的介绍。只有 [@oflyhigh 的一篇帖子里提到](https://steemit.com/cn/@oflyhigh/steemdata)，区块链的数据是实时同步到 steemdata 的。这令我更为困惑。于是，我就搜???了 steemdata 上的所有账号，发现最新的账号是 @asn191，创建于 2017-09-10 07:54:06 UTC。


> Why is ochedgreat, created on 2017-09-07, not in Steemdata? It seems not  a problem of time, but a problem of some missing data.


为什么创建于2017-09-07的 ochedgreat 不在 steemdata 上呢? 看起来不是个时间问题，而是数据丢失的问题了。


> In steemdata, @hannahwu loses nearly 200 followers, while @ochedgreat loses the identification. Shall I abandon steemdata and use steemsql instead? I would not like to, because many of my R scripts have been written to retrieve data from steemdata.com. But if it not reliable, all my data analysis are to be questioned, which is a disaster. 


在 steemdata 里， @hannahwu 丢失了将近 200 个粉丝，而 @ochedgreat 连自己的户口都丢了。我是不是该抛弃 steemdata，换用 steemsql？ 我不想这么做，因为我的很多R语言代码都是从 steemdata 获取数据的，我懒得改。但是，如果数据源本身不可靠，那么，我所有的数据分析都是可疑的，这无疑是个灾难。
