---
title: "@tvb 和 @tumutanzi 在一起，无图无真相 （兼谈一天里几点钟发帖最赚钱）"
author: dapeng
date: "2017-09-30 18:58:57"
slug: tvb-and-tumutanzi
categories: [cn]
tags: 
  - cn
  - steemswatch
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/tvb-and-tumutanzi), [cnsteem](https://cnsteem.com/cn/@dapeng/tvb-and-tumutanzi), [chainbb](https://chainbb.com/cn/@dapeng/tvb-and-tumutanzi), [busy](https://busy.org/cn/@dapeng/tvb-and-tumutanzi), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/tvb-and-tumutanzi.md)

![](https://cdn.pixabay.com/photo/2015/09/03/08/04/child-920128_960_720.jpg)

Image credit: Pixabay.com


总是有新朋友反复问同一个问题：在 steemit 的 cn 区发布文章，一天里到底几点钟发帖最赚钱？


对于这个问题，最直观的想法是：看看那些“**赚钱的文章发布在几点钟**”，不就行了嘛！


这好办。我们用万能的 R 语言，统计一下有史以来标有 cn 标签的所有帖子，共计 29518 篇，其中收益超过 100 SBD 的帖子的发布时间。见下图。


![high.png](https://steemitimages.com/DQmRo3JFZ6HN1Mc2TbfYT9MdcnVoTCJqvpBTGVMtqwCZXcb/high.png)


熟悉我写的“大鹏观察”系列帖子的朋友都知道，这是个24小时的时钟，每个扇形显示的是对应时刻发帖数量所占总数的百分比。很容易看出来，这些高收益的文章在 24 小时内都有，而在 12 时到 15 时（即北京时间 20 时 到 23 时）之间最为集中。


这下恍然大悟了吧：那就晚上发帖吧！


但是，——且慢！


下面是收益低于 10 SBD 的帖子发布时间分布图：


![low.png](https://steemitimages.com/DQmeDgXKm8VJ4aKWUpH7ywA6Ac8WTpCXq4bGycMW2S5Ms14/low.png)


怎么回事？低收益的跟高收益的差不多啊！也是晚上最集中！


再看看收益等于 0 的帖子：


![0.png](https://steemitimages.com/DQmfLYTw1aqVXnNWVuTMGu4cZmLh1JjfN261g4pwtZsdutk/0.png)


没错，也是集中在晚上！晚上发帖，高收益和低收益都有可能，甚至可能没收益！


问题出在哪里？出在逻辑上：“**赚钱的帖子发布在几点**”跟“**发布在几点最赚钱**”是**完全不同**的两个问题！


为什么都集中在晚上呢？因为 cn 区发帖的作者，不管大鲸还是小鱼??都是集中在晚上活动啊！下图是所有帖子的分布（该图在“[Steem 中国策 前传: 2016.07 - 2017.08](https://steemit.com/cn/@dapeng/steem-2016-07-2017-08-steem-s-watch-tcn0) ”现身过）：


![all.png](https://steemitimages.com/DQmQKcdacAYx5EUywcqycfhihZuTWtMvHQJd5xXePw4iUnx/all.png)


那么，如果我们把上图的每个扇形里，按照收益大小区分一下颜色，比如 0 -- 30 SBD 用蓝色， 30 -- 60 SBD 用绿色， 60 -- 90 SBD 用橘色，> 90 SBD 用红色表示，是不是就可以发现一些秘密呢？


![all_color.png](https://steemitimages.com/DQmPrXEvgjjhHEetYc8jo3ejGRpvMnbV19WvffrSG8x58sM/all_color.png)


肉眼看分布，其实各小时都差不多。仔细比较的话，0 时到 4 时（即北京时 8 时到 12 时）发布的帖子里，收益超过 30 SBD 的文章数 比其他时段略大一些。这似乎说明一条结论：上午发帖容易收益高。


遗憾的是，这个结论一点用都没有。这是所有人所有帖子混合起来的结果。而现实却是，别人上午发帖收益高，你未必。


这话怎么讲？


故事讲到这里，终于可以有请本文的女主角  @tvb 和男主角 @tumutanzi 出场了。


如果 @tvb 和 @tumutanzi  在一起，得到的图的真相是这样的：


![both.png](https://steemitimages.com/DQmQyKSGpSQ5wykz6ZUxT5g2dviteFfWqDDPAweeMvkTnRu/both.png)


发布在 12时、14时和22时的帖子里， > 90 SBD 的比例最高。那么对于 @tvb 来说，是不是只要选择在这几个黄金时段发帖就能赚大钱了呢？我们单独看看 @tvb 的帖子：


![tvb.png](https://steemitimages.com/DQmeLRyW3mGS6wfPpUtJUr2zeH1uE4KCHDP5VTpRhGH7Ly5/tvb.png)


22 时的黄金时段，跟 @tvb 没有半点关系。倒是 12 时和 14 时比较吻合，但这仅仅是巧合罢了，因为我们单独看看 @tumutanzi 就知道了：


![tumu.png](https://steemitimages.com/DQmRqXtZ24FBxEDTifoJT3BexNUh5dtfsocBe7twKXJKLfr/tumu.png)


12 时跟 14 时的高收益文章，几乎全部??自 @tumutanzi 的贡献！


所以，前面这三万篇帖子的收益统计分布，很大程度上，是受 @tumutanzi 这种影响力大的人所影响的。


是时候给出结论了：别琢磨几点发帖能赚钱了。文章收益跟发文时间的关系，完全可以忽略不计。影响力大的人，几点发帖都赚钱; 如果发帖不赚钱，不是因为发帖时段不对，而是作者的影响力不够大。要想提高影响力，两条路：好好创作优质文章，或投资买 SP。


可能有朋友会坚持：那么我只看我自己的数据不就行了？


不行的。你的影响力也在变化。数据只反映过去，不反映未来。除非建立个模型来预测，否则，得出的结论没有意义。


幸运的是我，赶在 @tvb 影响力爆发的前夜，做出了上面的图。让我们期待 @tvb 影响力的大爆发，将来再看她跟 @tumutanzi 在一起的模样吧！


PS: 本文属于["Steem 史记"](https://steemit.com/cn/@dapeng/steem-tvb) 的番外篇。Steem 史记，steem 之绝唱，无韵之离骚。



![大鹏](https://steemitimages.com/DQmeYUwQ7Juorgd79o6D5E34BnUYxwfmLxYH4cApgPRhRf6/end2.jpg)
