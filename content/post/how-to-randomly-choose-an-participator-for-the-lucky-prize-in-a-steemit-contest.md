---
title: "如何在 steemit 竞赛活动里认真抽取幸运奖 -谷哥点名#10  (How to Randomly Choose a Participator for the Lucky Prize in a Steemit Contest)"
author: dapeng
date: "2017-10-07 13:18:06"
slug: how-to-randomly-choose-an-participator-for-the-lucky-prize-in-a-steemit-contest
categories: [cn]
tags: 
  - cn
  - contest
  - programming
  - cran
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/how-to-randomly-choose-an-participator-for-the-lucky-prize-in-a-steemit-contest), [cnsteem](https://cnsteem.com/cn/@dapeng/how-to-randomly-choose-an-participator-for-the-lucky-prize-in-a-steemit-contest), [chainbb](https://chainbb.com/cn/@dapeng/how-to-randomly-choose-an-participator-for-the-lucky-prize-in-a-steemit-contest), [busy](https://busy.org/cn/@dapeng/how-to-randomly-choose-an-participator-for-the-lucky-prize-in-a-steemit-contest), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/how-to-randomly-choose-an-participator-for-the-lucky-prize-in-a-steemit-contest.md)

> It is easy to randomly choose a participator for a lucky prize in reality: use a dice, or write each participator's name on a slice of paper, mix them, and choose one, in public. It is not easy to do it in a Steemit contest. How can you show the dice or the chosen slice of paper to public and everyone believes you and thinks that it is fair? See the R scripts in this post and you will get the best-ever solution.


昨天公布的希望工程[新人"三个一"活动](https://steemit.com/cn/@dapeng/welcome-prize-for-new-steemians)，新老用户都可以参加幸运奖的抽取，而抽选方法并未公开。不是为了保密，而是因为这部分比较偏技术，而且篇幅长，怕喧宾夺主。本文详细说说，如何在一场 steemit 的竞赛中，以认真的态度随机挑选幸运奖。


![](https://cdn.pixabay.com/photo/2016/11/20/08/12/dice-1842135_960_720.png)


在现实中，随机抽取幸运奖的方法很简单：每个名字写到一个纸团里，混匀，**当众**随便拿一个出来就行了。如果不超过 6 个，**当众**掷一次骰子就行。这跟编程实现的效果是等同的。例如，R 语言里有现成的随机选择代码。我们暂且用 31 活动的赞助名单，来举个例子。


```

names <- c('victory622', 'tvb', 'shenchensucc', 'wangwenjing', 'drunkevil', 'dapeng')

n <- length(names)

```


n 表示参加人数。从 n 里随便选 1 个，只需运行：


```

names[sample(n, 1)]

```


完事儿。


但是，这个方法的致命缺陷是：**当众**。我说我运行代码的结果是 dapeng，谁信啊！没人亲眼看见我的运行结果啊！别说别人，我自己重新再运行一次，结果可能就变了呀！如果奖金额度小，可能大家不计较，万一是一笔巨款呢？谁知道是不是暗箱操作内定的？


所以，这个做法用在 steemit 的竞赛上，不够认真。


怎么做才算认真，才能服众？R 语言里早就考虑到这个问题了。为了实现可重复性，可以这样来：


```

names <- c('victory622', 'tvb', 'shenchensucc', 'wangwenjing', 'drunkevil', 'dapeng')

n <- length(names)

set.seed(31); names[sample(n, 1)]

```


前两行跟此前的代码完全相同。第三行先设置个种子，然后再随机选。这里，我们暂且给种子编号为 31。这样的话，不管啥时候，不管在哪台电脑上运行上面三行代码，都是同样的结果。免得大家怀疑主办方作弊，把幸运奖给内定了。如果你电脑上装了 R 语言，不妨试试上面的代码，看看结果是不是 wangwenjing。


由于参赛名单不到最后一刻谁都不知道，所以运行的结果没法事先内定。


也许还会有人质疑：你糊弄谁呢？我又不懂 R 语言，怎么检验你的结果？


这个也好办。即使不懂 R 语言，你也可以轻松检查上述代码的运行结果。随便访问个 R 语言在线网站，例如[这里](http://rextester.com/l/r_online_compiler)、[这里](http://www.r-fiddle.org/#/fiddle?id=IMMSu4Na)、或[这里](https://www.jdoodle.com/execute-r-online)，把上面那三行代码复制粘贴进去，点运行，就看到结果了。看看是不是 wangwenjing。


这已经是认真到万无一失了，但我们还可以更进一步，把事情做绝：将来抽奖的时候，我们把上面示例代码的种子编号 31，改为最后一位参加者发布文章时间的秒数，以区块链记录该文章的 created 时间为准。


好了，不到最后一刻，谁都不知道最终的实际参加人数，也不知道种子编号。哪位能提供更认真的方法吗？欢迎拿出来单挑。


至于“三个一”活动幸运奖最终花落谁家，让我们拭目以待。


![dapeng](https://steemitimages.com/DQmeYUwQ7Juorgd79o6D5E34BnUYxwfmLxYH4cApgPRhRf6/end2.jpg)
