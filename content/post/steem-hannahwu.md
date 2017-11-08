---
title: "Steem 史记： @hannahwu 列传"
author: dapeng
date: "2017-09-08 08:23:42"
slug: steem-hannahwu
categories: [cn]
tags: 
  - cn
  - blog
  - cn-blog
  - steemswatch
  - cn-reader
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/steem-hannahwu), [cnsteem](https://cnsteem.com/cn/@dapeng/steem-hannahwu), [chainbb](https://chainbb.com/cn/@dapeng/steem-hannahwu), [busy](https://busy.org/cn/@dapeng/steem-hannahwu), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/steem-hannahwu.md)

是的，大家没有看错，本期“大鹏观察 - Steem 史记”的主角，正是万众期待的—— @hannahwu！（停顿，此处观众可能会有长时间的掌声。）


@hannahwu, 江湖人称“狼姐姐”。千呼万唤始出来，我特别制作了一张图。这是个词云图，是狼姐姐帖子里出现的关键词。字符越大，在狼姐姐帖子里出现次数就越多。所以，这是狼姐姐在 Steemit 发文的“指纹图”。所有关键词组成的轮廓，是一匹狼，一匹嗷嗷叫的狼。大家感觉如何？跟狼姐姐的形象匹配吗？


[![](https://steemitimages.com/DQma9ULTms89jkrCjvwvCcntLBa6Tj1DVXbWbokqYD4C3Vy/a8-1.jpeg)](https://steemitimages.com/DQma9ULTms89jkrCjvwvCcntLBa6Tj1DVXbWbokqYD4C3Vy/a8-1.jpeg)


受页面限制，图有点小，点击它就可以看大图了。


这是“大鹏观察”的一次升级。以后，凡是报名参加本活动的主角，都可以指定一张你喜欢的图片，我可以把帖子关键词做成你要的模样，就像这张狼图。


以往的“steem史记”，封面图片默认是主角profile里的图片。上期活动，默认用了 @mrspointm 的照片做封面，被我老婆看见了，我一顿解释，哎......不说了，说多了都是泪......以后，统统用指纹图作为帖子的封面图片。


需要注意的是，指纹图的图片要求是背景透明，不透明的部分将被关键词填充。如何制作背景透明的图片，可以参考我的帖子[Powerpoint 制作你的专属 Steemit 透明背景水印](https://steemit.com/cn/@dapeng/steemit-tips-create-your-steemit-watermark-using-powerpoint-steemit) 。也可以 google 搜索网上现成的图片，在搜索结果的工具选项里选择“透明”即可。


除了词云图形状升级之外，以前关键词的统计有些问题，因为很???无意义的词也统计在内了。在 @deanliu 前辈的建议下，从本期开始增加关键词过滤功能（stopwords），把一些无意义的词删掉了。即便如此，仍有一些漏网之鱼——中文的组合太复杂了，大家先凑合着看吧。


包括狼图制作在内，本文的数据获取、分析、图表制作、报告编写全程使用仍然是人见人爱的 R 语言，数据来源是 steemdata.com。


看了狼姐姐的数据后，我们发现两件怪事：


1.  八月中旬，狼姐姐既没有点赞，也没有评论，更别提发帖了。是一片空白，就像小龙女藏到了绝情谷底。

2.  一般人是 0 时到 8 时之间休息，不发帖，而狼姐姐是在 2 时到 10 时之间从未发过帖，仿佛生活在新疆。


这是为什么？你猜。


---


*前情回顾*:


- Steem 史记： [@tumutanzi](https://steemit.com/@tumutanzi) 世家([1](https://steemit.com/cn/@dapeng/steemit), [2](https://steemit.com/cn/@dapeng/steem-a-preliminary-analysis-of-a-steem-id-s-data), [3](https://steemit.com/cn/@dapeng/no-1s-of-his-steem-posts-steem))

- [Steem 史记： @justyy 列传](https://steemit.com/cn/@dapeng/steem-id-report-1-justyy-1)

- [Steem 史记： @htliao 列传](https://steemit.com/cn/@dapeng/steem-htliao-steem-s-watch-a2)

- [Steem 史记： @shenchensucc 列传](https://steemit.com/cn/@pzhao/steem-shenchensucc)

- [Steem 史记： @mrspointm列传](https://steemit.com/cn/@dapeng/steem-mrspointm)


“Steem 史记”系列需要你的参与，报名方式为： **自荐。如果希望下下一期（因为下一期已经有人选了）对你自己的用户数据进行分析，那么在最新一期的“Steem 史记”上点赞（Upvote）和留言（Reply）即可。被顶次数最多、位置最靠上的 ID，将是我们下下一期的故事主角。**


---


## Steem 史记： @hannahwu 列传


 @hannahwu 者， 不知何方人氏，貌似常在苏州。由于本文涉及的时间均采用标准时区 UTC，换算成该时区均???加上 8 小时。


话说那是个载入史册的时刻： 2017-07-09 03:17:15。乾坤混沌，天地苍茫，每个人都不知道 steem 未来的方向在哪里，不知何去何从。就在这时，某个角落，传来一声婴儿的响亮啼哭。 作为这个世界的第 249952 个生命，@hannahwu 降生了。


光阴荏苒，如今已是 2017-09-06 14:36:11, Steem 全网注册用户总数已有 341491 个，全网发帖总数已经有 2025202 篇。在这茫茫人海里， @hannahwu 有过哪些壮举和作为？


This is a report of the Steemit ID @hannahwu. The data were sampled from https://steemdata.com/ at 2017-09-06 14:36:11, when there were in total 341491 accounts and 2025202 posts on Steem. Data were processes and this report was written in R

 language.



### @hannahwu 的基本信息 Profile



| items           | info                                     |
| :-------------- | :--------------------------------------- |
| name            | hannahwu                                 |
| id              | 249952/341491                            |
| created         | 2017-07-09 03:17:15                      |
| profile_image   | ![](https://steemitimages.com/0x0/https://steemitimages.com/DQmakBbB7qXDEVYRii5SMMUsQWFg6gRegHbYHSrzhww93XL/about.jpg) |
| about           | Hannah，水瓶座，爱花，爱生活，爱田园，喜欢亲近大自然，喜爱小动物，爱好摄影。 |
| location        | N.A.                                     |
| website         | https://www.hannahwu.com/                |
| post_count      | 981                                      |
| available_STEEM | 0                                        |
| available_SBD   | 56.831                                   |
| available_VESTS | 1725461.75161                            |
| reputation      | 12731395804795                           |
| followers_count | 227                                      |
| following_count | 165                                      |



### 帖中之最 Top Posts


???诞生后，@hannahwu 就对这个世界发出了自己独特的声音，共发帖 73 篇。我们来看看 @hannahwu 发布的帖子里的几个第一名。


In this section we listed @hannahwu's top posts.


**字符最多的帖子 Top post with the most characters.**


- [玉龙雪山，四千米处撒欢 Yulong Snow Mountain, Ski at 4000 Meters above Sea-level](https://steemit.com/@hannahwu/yulong-snow-mountain-ski-at-4000-meters-above-sea-level)，含 5601 个字符。


**插图最多的帖子 Top post with the most figures.**


- [玉龙雪山，四千米处撒欢 Yulong Snow Mountain, Ski at 4000 Meters above Sea-level](https://steemit.com/@hannahwu/yulong-snow-mountain-ski-at-4000-meters-above-sea-level)，含 32 张图片。


**修改间隔最长的帖子 Top post with the longest time between the publication and the final edit.**


- [Embrace Steemit at my 6th Blogoversary!! 博客六周年之际来一篇Steemit安利](https://steemit.com/@hannahwu/embrace-steemit-at-my-6th-blogoversary-steemit)，发布 41.2 小时即 1.7 天之后，作者做了最后一次修改。


**得票数最多的帖子 Top post with the most upvotes.**


- [Selfportrait Contest 自画像](https://steemit.com/@hannahwu/selfportrait-contest)，得到 109 个赞。


**赚钱最多的帖子 Top post with the most payout value.**


- [祖辈爱情（三）：最美好的初恋≠最终的归宿](https://steemit.com/@hannahwu/5uhqtm)，收入为 94 美元。





### 粉丝情况 Followers and following


@hannahwu 广结四海豪杰，有 227 个追随者，@hannahwu 关注的 ID 总数是 165。其中，有 47 个 ID 跟 @hannahwu 是双向关注的，而 118 个ID 虽然被 @hannahwu 关注，但却没有关注 @hannahwu 。


@hannahwu had 227 followers. @hannahwu followed 165 ID in total, in which 47 IDs interacted with @hannahwu bidirectionally, while 118 IDs did not follow @hannahwu.


![a9-1.png](https://steemitimages.com/DQmes7uLMw53HPoCsyUMEmMYRcnVNiB4e5X3ncyyNVhWB9A/a9-1.png)





若问上图中红色和蓝色区域的名单，请使用 @dapeng 开发的[在线小工具 steemr](https://steemit.com/cn/@dapeng/steemr-a-web-based-tool-for-steemers-or-steemians-steemr)。


随着朋友数量的变化， @hannahwu 逐渐积累声望。下面是声望值增长的时间趋势。


![a10-1.png](https://steemitimages.com/DQmXqKTMsEJ4cbHGnRYRyofRsw8gMyCzwFDhg7bWB9xzdm1/a10-1.png)


### 发帖 Posts


下图是 @hannahwu 的发帖时间图，图里每个点代表一篇帖子，往左水平看对应的是发帖的时刻，往下垂直看是发帖的日期。图中使用的标准时区 UTC。


The following figure shows @hannahwu's active time. The green line indicates @hannahwu's register time on Steem.


![a11-1.png](https://steemitimages.com/DQmeVuRfPeP5FqUyn1APRdzZHPaGgSJfh42oRFMz8itV4Ro/a11-1.png)



下图是个特殊的时钟，一圈是24小时，显示了 @hannahwu 一天24小时里发帖的频次，面积越大的时段，发帖数就越多。红线显示的是频次分布：每两条相邻红线之间的帖子数，占全部帖子数的 25%。哪两条红线最接近，哪两条红线之间就是  @hannahwu 发帖的高峰时段。主要集中在北京时间 13  时和 0 时。北京时间 2 时到 10 时之间从未发帖，很有规律。


The figure below shows the frequency of @hannahwu's posts. 



![a13-1.png](https://steemitimages.com/DQmZMTDnukom4Nn93JDXnczLLQFbWQUxihTz4JyANSeyY1r/a13-1.png)



下图是每周累计发帖总数。


![a14-1.png](https://steemitimages.com/DQmPgQuCDPXpzVbBUS4q6xwT8kc48zHF3Lry8x2mBkHc6eL/a14-1.png)



### 留言 Reply


下图是 @hannahwu 对别人帖子的评论（留言）时间图。蓝色点表示周一到周五，红色表示周六和周日。八月中旬好像发生了什么。



![a15-1.png](https://steemitimages.com/DQmaFBgNrVAVWG64NuKwQfgdzRFEDN6EfHDSGAN4A6qdr3W/a15-1.png)


下图是 @hannahwu 每天发布评论的时刻统计。24 小时全有？


![a17-1.png](https://steemitimages.com/DQmUXMYrhCnxH24eiUYfdUGR3wn9BtdwuaVCwyrRobLtgqi/a17-1.png)


下图是每周发表的评论总数。


![a18-1.png](https://steemitimages.com/DQmPuy2YGqKuCTWmTrkSxGf5DLt8ZzDssvsKbg8A5hEfyNo/a18-1.png)


### 点赞 Vote


下图是 @hannahwu 发布投票（点赞）的时间趋势图。


The following figure shows @hannahwu's active vote time. 

![a19-1.png](https://steemitimages.com/DQmTCS6XT26VyCgpe3Yurb3A3z7GnGVPtgRC8Te6AuDNCR1/a19-1.png)



下图是 @hannahwu 点赞的24小时分布图。24小时全有？



![a21-1.png](https://steemitimages.com/DQmenrjuMtQ6J6osFXSS3HzuPAhipQvFvaVoETD69Cf5Zog/a21-1.png)



每周点赞总数：


![a22-1.png](https://steemitimages.com/DQmPisRfs3GkSdjYx2qRu8XvuZhdLTZ2K39hfBiFTiyEkvE/a22-1.png)



### 帖子的质量和收入 Quality and money



下面的数据表格是 @hannahwu 发帖的首选分区的次数。@hannahwu 发帖最多的圈子是 'cn'。


The table below shows the categories (the first tags) of @hannahwu's posts. @hannahwu posted most posts in 'cn'.




| category             | Freq |
| :------------------- | ---: |
| cn                   |   71 |
| food                 |    1 |
| selfportrait-contest |    1 |



现在我们来谈谈钱。下图显示的是单篇帖子收入的分布。横坐标是美元，阴影面积越大，对应美元的帖子数量越多。 @hannahwu 共发帖 73篇，总收入为 1377.76 SBD， 单帖收入最高为94.47 SBD，平均每帖收入为18.87 SBD。一半的帖子收入都在 34 SBD 以上。


Now let's talk about money. The figure below shows the dollars @hannahwu got from each post. Averagely @hannahwu earned 18.87 dollars per post, with the maximum of 94.47 dollars from one post.



![a25-1.png](https://steemitimages.com/DQmQfcLEv2zfBLiXQzR2MKagrKdTCf6PmFjCNXTeHZWoxWm/a25-1.png)



下图显示的是每帖收入的时间趋势。


The figure below shows the trend of @hannahwu's money per post.


![a26-1.png](https://steemitimages.com/DQmXERevhggEWdvi6s17voy7oKYR4WYkhLcJfoeyyMbpMxQ/a26-1.png)


下图是 @hannahwu 帖子获得???投票（点赞）数。 @hannahwu 累计得赞 2776  个，单帖得到的点赞数最高为 109 个，平均每帖得赞 38  个。


The figure below shows the upvote number of each post. Averagely @hannahwu earned 38 upvotes per post, with the maximum of 109 upvotes.


![a27-1.png](https://steemitimages.com/DQmW1euQSRAKkwJYXt2DEbUqZ9XCfzgvhQfBUu5zaEbMs1M/a27-1.png)


下图是平均每赞得到的收益 SBD 的时间趋势。


![a28-1.png](https://steemitimages.com/DQmSocPNNv5ogz55eXBu9LmR5V7TuTEnAe2DKudGbLUEG8j/a28-1.png)


下图是每周收入总和的时间趋势。


![a29-1.png](https://steemitimages.com/DQmXf2AoMVDio8LaCfex7ZUXKT8dU3RFHcwm3xQum5K1CNd/a29-1.png)


为 @hannahwu 帖子得到的投票次数最多的前三位伯乐是  @tumutanzi, @herlife, @jessicameng。下面为 @hannahwu 帖子得到的投票次数超过 20 次的 ID 词云图。


![a30-1.png](https://steemitimages.com/DQmW6xSazE2Y9k2msDF9crTCjLG73EVjLCneQavLRsfv8kZ/a30-1.png)



为 @hannahwu 帖子收益贡献最多的前三位伯乐/金主/贵人是 @abit, @tumutanzi, @linuslee0216。他们一共贡献了 @hannahwu 全部收入的 79%。排在他们后面的第 4 到第 10 位的贡献比例如下图。


![a31-1.png](https://steemitimages.com/DQmcfqooYGRfNvyh6YnKk3pTEh3bEBM3QgUHaYrGXqXaCjt/a31-1.png)

---



感谢关注“大鹏观察”。欢迎参加下一期的活动，也欢迎提出宝贵意见。谢谢。


![steeemswatch_dapeng.jpg](https://steemitimages.com/DQmbKrfakkprV9jDF6nr4akB25gdq4qQm5dRr8GkGNUS9Gy/steeemswatch_dapeng.jpg)



Tags: #blog #cn-blog #steemswatch #cn-reader
