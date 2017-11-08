---
title: "看到他暴露的 Steem 用户数据后我震惊了 a preliminary analysis of a steem ID's data"
author: dapeng
date: "2017-07-31 10:14:24"
slug: steem-a-preliminary-analysis-of-a-steem-id-s-data
categories: [cn]
tags: 
  - cn
  - blog
  - steem
  - steemit
  - r-language
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/steem-a-preliminary-analysis-of-a-steem-id-s-data), [cnsteem](https://cnsteem.com/cn/@dapeng/steem-a-preliminary-analysis-of-a-steem-id-s-data), [chainbb](https://chainbb.com/cn/@dapeng/steem-a-preliminary-analysis-of-a-steem-id-s-data), [busy](https://busy.org/cn/@dapeng/steem-a-preliminary-analysis-of-a-steem-id-s-data), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/steem-a-preliminary-analysis-of-a-steem-id-s-data.md)

In my previous posts ([1](https://steemit.com/steemit/@dapeng/new-steemians-have-you-have-thought-about-your-data-privacy), [2](https://steemit.com/cn/@dapeng/steemit-two-weeks-on-steemit-rather-a-social-platform-than-a-writing-tool)), I talked again and again about steem users' data. Sorry that I am not good at talking, and maybe some do not know exactly what I was talking about. In this post, I will show you what information you can get out of any steem ID. Yes, anyone like me can get such information easily, even he/she knows nothing about hacking skills. **Think twice before you do something on Steem.**


Thanks to @tumutanzi for his generosity of letting me use his data as an example. 



在前两篇帖子里（[1](https://steemit.com/cn/@dapeng/steemit), [2](https://steemit.com/cn/@dapeng/steemit-two-weeks-on-steemit-rather-a-social-platform-than-a-writing-tool)），我反复强调了 steem 用户的个人数据，并且开发了个[小工具 steemr](https://steemit.com/cn/@dapeng/steemr-a-web-based-tool-for-steemers-or-steemians-steemr)，方便大家查阅其中的部分数据。 @tumutanzi 嫌[口味不够重](https://steemit.com/cn/@dapeng/steemr-a-web-based-tool-for-steemers-or-steemians-steemr#@tumutanzi/re-dapeng-steemr-a-web-based-tool-for-steemers-or-steemians-steemr-20170727t162813885z)。别急，那只是开胃小菜，好吃的都在后头，让我们渐入佳境。这次稍微加点佐料，我们对 @tumutanzi 的发帖数据进行进一步深挖，看看能八出什么秘密。


注意，我不是黑客，任何用户的这些数据都可以轻易得到，根本不需要任何黑客技术。所以，**请你注意自己在 steem 上的一举一动**！我对你的个人隐私没有兴趣，但这并不代???别人对你也没有兴趣，而别人的技术和分析手段可能比我高明得多！


![](http://yaeckerdesign.com/wp-content/uploads/Tell-You-The-Secret-To-Maintain-Wedding-Gowns-yrqEpo.jpg)


Figure source: http://yaeckerdesign.com


## His active time 活跃时间


The following figure shows his active time. The green line indicates his register time on Steem.


下图是他自注册以来的发帖时间图，图里每个点代表一篇帖子，水平往左看对应的是发帖时间，垂直往下看是发帖日期，绿线是他在 steem 的注册时间。



![unnamed-chunk-2-1.png](https://steemitimages.com/DQmcTM5RxGavjgjAzpt1drRXm23LFQ5hzawshYvDRi9PWzB/unnamed-chunk-2-1.png)


Until July 30 2017, he had posted 78 posts. On the first day, he posted three posts. For some reason, there was a long break for three months in 2017. Afterwards, he became very active, especially in July 2017. Most of his posts were posted between 8:00 and 24:00, which might be his getting-up and going-to-sleep time.


截至2017年7月30日，@tumutanzi 发帖总数是 78篇。在注册当天下午，他就"Duang-Duang-Duang"连发三帖（上图绿线上的三个点。收入全是 0，详见下文）。在2017年3月以前，发帖断断续续。不知什么原因，他的发帖在2016年11月份有短暂中断，而在2017年连续中断了3个月，到7月份突然非常活跃。发帖的时间多在早上8点以后（UTC，下同）和0点以前，这可能是他的起床和就寝时间。他的作息时间是比较规律的。


![unnamed-chunk-3-1.png](https://steemitimages.com/DQmdK1K3w21pHzDCZMLmvrPrbp2ATgoZc3ye7UnjCYpwEtF/unnamed-chunk-3-1.png)



The figure above shows the frequency of his posts. There were 25% of the posts were posted after 22:00, and 50% after 17:00. He is active at night. That is why he wrote below his ID, 'Falling in love with Steemit and I have no time for X...'


上图显示的是他一天24小时里发帖的频次，横坐标是每天的几点钟。阴影面积越??的时段，发帖数就越多。 从图上看，有25% 的帖子都是 22:00 以后发布的，而50% 的帖子是在下午 17点以后发布的。晚上是坛子发帖的活跃期。难怪他的 ID 下面写着：“爱上Steemit后，X生活都没时间了……”


His attitude to posts 对帖子的态度

----------------------------------


![unnamed-chunk-4-1.png](https://steemitimages.com/DQmPQKtr74UsXiLwqWbWvD34Nu6RrBY9RSK9V6zppH1smtf/unnamed-chunk-4-1.png)


The figure above shows how many edits for each post. At the beginning, he editted most of the posts fewer than two times each. In July 2017, most posts were editted more than three times. On post was editted even 15 times! He is getting more and more careful with his words.


上图是每个帖子的编辑次数，图里每个点代表一篇帖子，水平往左看对应的是该帖被编辑的次数。 在刚刚进入steem的时候，他发帖以后修改的次数比较少，大部分在每帖2次以下。而进入2017年7月以后，修改次数明显增多，大部分帖子都修改3次以上，修改最多的次数达到了15次之多。反复修改说明他对自己的帖子精益求精。要知道，他长久以为只有24小时内才能修改，如果他知道7天之内都能修改的话，修改次数可能更多。


| category            | Freq |
| ------------------  | --- |
| bitcoin             |    1 |
| cn                  |   62 |
| education           |    1 |
| electric-toothbrush |    1 |
| hiking              |    1 |
| imagej              |    1 |
| luck                |    1 |
| make-money          |    1 |
| revolut             |    1 |
| smart-tv            |    1 |
| sports              |    1 |
| steemit             |    1 |
| talented            |    1 |
| tech                |    3 |
| uk                  |    1 |


The table above shows the categories (the first tags) of his posts. He posted most of them in CN.


上面的数据是他发帖的首选分区的次数。虽然身在海外，但他把???的青春绝大部分都奉献给了他的家乡：CN区。鼓掌！


## Quality and money 帖子的质量和收入


![unnamed-chunk-6-1.png](https://steemitimages.com/DQmTMZQv2Wo6rradTGXncVMD5fkrmuFHFBQ1mJ7FMji4MQX/unnamed-chunk-6-1.png)


Now let's talk about money. The figure above shows the dollars he got from each post. Averagely he earned 27.03 dollars per post, with the maximum of 191 dollars from one post. However, half of his posts had a value below 6 dollars. A quarter of them even were less than 1 dollar. He used to be a rookie as well as you and me.


现在我们来谈谈钱。上图显示的是单篇帖子收入的分布。横坐标是美元，阴影面积越大，对应美元的帖子数量越多。 @tumutanzi 现在动不动就每帖收入近百美元，单帖收入最高为191美元，平均每帖收入为27.03 美元。但是，有一半的帖子收入都在6美元以下；25% 的帖子，收入不到1美元。而75%的帖子带来的收入都不足45美元。他也是从菜鸟过来的呀。


![unnamed-chunk-7-1.png](https://steemitimages.com/DQmZUzWtuGW6RFxrjBSTg1rdfFztNFJ5NCRpKB8tfCC9cBm/unnamed-chunk-7-1.png)



His posts have a long-life time. Most of them still attracted comments 63 hours or 2.6 days after posted. Somebody even commented on one of his post after 8021 hours 334 days! Well done!


他的帖子生命力很顽强，有半数以上的帖子在发布63小时即2.6天后仍然有人在帖子后面留言。有的帖子，在发布8021小时即334天后，仍然有人评论。好样的！

![unnamed-chunk-8-1.png](https://steemitimages.com/DQmagwbmTZedfWDQRvp6K7qmac3KDwBstskd7eoFWLaokKo/unnamed-chunk-8-1.png)


The figure above shows the trend of his money per post. At the beginning, each post gave him no money. After three months, he got 10 dollars per post. It increased sharply in July 2017. So just keep writing good posts and money will come to you.


上图显示的是每帖收入的时间趋势。早期的帖子收入很多都在0附近徘徊。坚持三个月???，单帖收入到了10美元左右。到了2017年7月陡增。一方面，即使像 @tumutanzi 这样的优秀博主写的好帖子，有个别帖子到现在也难逃低收入的厄运：另一方面，大部分的优质帖子还是得到了丰厚的回报的。所以新手们不要沮丧，坚持写，写好帖，你的收入会像他这样上升。我们往往羡慕别人今天的成就，却忽视他曾经走过的路，忽视他昨天付出的艰辛和努力。


![unnamed-chunk-9-1.png](https://steemitimages.com/DQmQSYQaGPowkdzwQzvJbUGLMqAyroVTzNGwELfqdHyNjqQ/unnamed-chunk-9-1.png)


The figure above shows the upvote number of each post. Although he was more active in July 2017 than before, his upvote number seemed not larger. Let's look forward to his future trend!


上图是坛子帖子获得的投票数。虽然7月份发帖比较活跃，但是单篇的投票数并没有比去年12月多多少。 @tumutanzi，加油！



If you are interested in your own ID, please upvote this post and leave a comment, and I will post the figures of you!


最后，如果有哪位想对自己的 ID 数据进行上述分析，请 upvote 本帖并留言，我可以把分析图表贴出来。仅限自己的 ID 哦！如果要查的人太多，我就把这个功能放到我的[小工具 steemr](https://steemit.com/cn/@dapeng/steemr-a-web-based-tool-for-steemers-or-steemians-steemr)里，只需输入个目标 ID，每个人就可以想查谁就查谁，大家说这样好不好？


To be continued ......

*未完，待续......*
