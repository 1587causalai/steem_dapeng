---
title: "steemsql 也开始不靠谱了"
author: dapeng
date: "2017-10-30 09:49:27"
slug: steemsql
categories: [cn]
tags: 
  - cn
  - cn-programming
  - steemsql
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/steemsql), [cnsteem](https://cnsteem.com/cn/@dapeng/steemsql), [chainbb](https://chainbb.com/cn/@dapeng/steemsql), [busy](https://busy.org/cn/@dapeng/steemsql), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/steemsql.md)

今天的“希望工程”日报一出来，我就发现新人新帖里很多垃圾文，没有经过过滤。


我有个小号 @pzhao ，当作机器人来用，打算自动发布一些模板化的帖子和评论。目前，”历史上的今天“已经交给机器人发布了。我一直想等着“希望工程”日报做成熟之后，也交过去，免得对我的一些 followers 造成骚扰。可是，除了 steem python API 经常发不出去文章之外，还时不时出点别的幺蛾子。steemsql 就是一个。


“希望工程”日报的垃圾帖过滤工作，是用 R 语言程序完成的。R 程序自动从 steemsql 数据库里，读取 @incrediblesnow 最新发布的 cn-abuse 报告，从中获取新增的灰名单和黑名单，然后对新人新帖进行过滤。


然而，[昨天的 cn-abuse 报告](https://cnsteem.com/cn/@incrediblesnow/29-10-2017-cn-abuse-report-for-cn-abuse-on-29-10-2017)，在 steemsql 里看不见。例如搜索：


```

SELECT body 

FROM Comments 

WHERE title like N'%Cn-abuse 的报告%' 

  AND author = 'incrediblesnow' 

  AND json_metadata like '%\"cn\"%' 

  AND created BETWEEN '2017/10/29' and '2017/10/30'

```


结果是零条。


放宽一下搜索条件：


```

SELECT title 

FROM Comments 

WHERE author = 'incrediblesnow' 

  AND created BETWEEN '2017/10/20' and '2017/10/30' 

  AND title <> ''

```


仍然搜不到。


![steemsql.jpg](https://steemitimages.com/DQmT2EerJQhoLsMUTQEKzCfgQiQ8vhnRH4etzrFU2gZ8Va3/steemsql.jpg)


这就导致昨天的灰名单和黑名单没有被读到，所以“希望工程”的日报就没有得到过滤。好在，就算是没过滤，新人新帖也比前些天大为减少了。


两个月前，我发现 [steemdata 的数据框不靠谱](https://steemit.com/cn/@dapeng/unreliable-analysis-on-steem-data-steem)，于是换到了 steemsql。现在连 steemsql 也不靠谱了，该怎么办？





![dapeng](https://steemitimages.com/DQmeYUwQ7Juorgd79o6D5E34BnUYxwfmLxYH4cApgPRhRf6/end2.jpg)
