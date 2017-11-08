---
title: "大鲸和小鱼等级计算方法的建议  Suggestions on Definition of Small Fishes and Big Whales on Steemit"
author: dapeng
date: "2017-09-29 08:30:09"
slug: definition-of-small-fish-and-big-whale-on-steemit
categories: [cn]
tags: 
  - cn
  - steemit
  - steemitboard
  - steem
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/definition-of-small-fish-and-big-whale-on-steemit), [cnsteem](https://cnsteem.com/cn/@dapeng/definition-of-small-fish-and-big-whale-on-steemit), [chainbb](https://chainbb.com/cn/@dapeng/definition-of-small-fish-and-big-whale-on-steemit), [busy](https://busy.org/cn/@dapeng/definition-of-small-fish-and-big-whale-on-steemit), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/definition-of-small-fish-and-big-whale-on-steemit.md)

严格来讲， steemit 并没有“大鲸”和“小鱼”。


Steem 上“鲸”和“鱼”的分级来自 [steemitboard](https://steemitboard.com/) ，将用户分 5 级，从小到大依次是：红鱼，米诺鱼，海豚，杀人鲸，鲸。你看，里面根本没有“大鲸”和“小鱼”的说法。后者只是俗称。


那么，这5级是怎么定义的？


> The title of this post is technically wrong. There is neither small fish nor big while. Five levels of steemians were given by  [steemitboard](https://steemitboard.com/). They are red fish, minnow, dolphin, orca, and whale. They are defined according to the  vesting shares of the account. 


是根据用户的 vesting_shares 定义的。如果用户的 vesting_shares 少于 1000000（6个零，即 1 M）， 那就是红鱼；多于 1000000000（9个零，即1 G），就是鲸。介于两者之间，每多个零，就升一级。也就是说：


```

红鱼 < 1M < 米诺鱼 < 10M < 海豚 < 100M < 杀人鲸 < 1G < 鲸

Red fish < 1M < Minnow < 10M < Dolphin < 100M < Orca < 1G < Whale

```



那么，vesting_shares 是什么？


其实就是 Steem Power （SP，即“权力”）换算成另一个单位而已，中间需要一个由区块链内部定义的常数，叫做  steem_per_mvests，可以在 [steemd](https://steemd.com/) 网页右上角看到，目前的值是 485.668。每 1 M 的 vesting_shares，约等于486 个 SP。


```

Steem Power =  vesting_share * 485.668 / 1000000

```


这样一换算，就很容易通过权力（SP）来判断等级了：


> As the Steem Power (SP) is calculated from the vesting power and the steem per mvests (485.668, which can be found on [steemd](https://steemd.com/)), we can define the user level by SP:


```

红鱼 < 486SP < 米诺鱼 < 4860SP < 海豚 < 48600SP < 杀人鲸 < 486000SP < 鲸

Red fish < 486SP < Minnow < 4860SP < Dolphin < 48600SP < Orca < 486000SP < Whale

```


为了方便，这里只取三位有效数字，并忽略科学记数法的问题。


米诺鱼是一种小型鲤鱼，红鱼是一道好菜。这些名称不够直观。结合大家的惯用法，我建议在中文区把他们叫做：小鱼，大鱼，海豚，小鲸，大鲸。


所以，更简单来说， SP 高于5百，就是大鱼；5千，海豚；5万，小鲸； 50 万，大鲸。


> I think these names are too complicated to steemians, especially to those who know nothing about zoology or have never been to a sea. For simplicity, I would call them small fish, big fish, dolphin, small whale, big whale.

>
> I think it is unfair to define the level by SP. ESP makes more sense. BTW, On steemiboard, a user with no activity is marked as dead fish. It is unfair as well. On the name list of CN community,  user levels are given according to ESP, and nobody is dead fish. After all, dolphins and whales are mammals. They are not fishes at all!


![level.jpg](https://steemitimages.com/DQmasoQQNTKQpSBb96y4QQ9o5sPhiF8tjPX7YG4dCL3axc1/level.jpg)


然而，如果你用 [steemitboard](https://steemitboard.com/) 查某个用户的等级，例如[查询有“临时大鲸鱼”美称的 @tumutanzi](https://steemitboard.com/@tumutanzi)，却发现他只是个海豚；而[一哥 @myfirst](https://steemitboard.com/board.html?user=myfirst) 更离谱，是条死鱼。这是怎么回事？


因为 @tumutanzi 有 50 万的权力来自 ned 的代理 ，从而“实权”(即有效权力，Effective SP，ESP) 达到了大鲸的等级。“临时大鲸鱼”这个名称是我最先叫出来的，灵感来源于孙中山先生的“临时大总统”一职。按照 ESP 来分等级的话，我们还可以称呼某个人“临时小鲸”，"临时海豚"等。


而 @myfirst ，只要最近 7 天没活动，就被 steemitboard 标为死鱼。


既然 ESP 比 SP 更具有现实意义，那么 steemitboard  用SP 算等级就显得不合理了，而7天不活动就标死的做法更是不近人情。我认为应该按 ESP 来算。所以，在 [Steem 中文区水浒英雄排行榜](https://steemit.com/cn/@dapeng/6mnla8-steemit-cn)上，我新增了“用户等级”一栏，按 ESP 来显示用户属于哪一级。目前的 108 将里，有 5 条大鲸，4 条小鲸，8 条海豚，37 条大鱼，剩下的 54 条（恰好占一半）是小鱼。


来[排行榜](http://steemr.org/)看看吧，你属于哪种鱼？


PS：海豚和鲸其实都属于哺乳动物，不是鱼。 


![end.png](https://steemitimages.com/DQmWKRoZhpvHW3sFkHUnfkbZGNsZUe8FBEgEbkRXQXoE4bu/end.png)
