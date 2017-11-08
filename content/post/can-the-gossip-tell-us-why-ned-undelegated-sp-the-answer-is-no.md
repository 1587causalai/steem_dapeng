---
title: "Can the Gossip Tell us Why Ned Undelegated SP? The answer is no"
author: dapeng
date: "2017-10-27 15:44:27"
slug: can-the-gossip-tell-us-why-ned-undelegated-sp-the-answer-is-no
categories: [steemit]
tags: 
  - steemit
  - bisteemit
  - stats
  - news
  - cn
---

原文链接: [steemit](https://steemit.com/steemit/@dapeng/can-the-gossip-tell-us-why-ned-undelegated-sp-the-answer-is-no), [cnsteem](https://cnsteem.com/steemit/@dapeng/can-the-gossip-tell-us-why-ned-undelegated-sp-the-answer-is-no), [chainbb](https://chainbb.com/steemit/@dapeng/can-the-gossip-tell-us-why-ned-undelegated-sp-the-answer-is-no), [busy](https://busy.org/steemit/@dapeng/can-the-gossip-tell-us-why-ned-undelegated-sp-the-answer-is-no), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/can-the-gossip-tell-us-why-ned-undelegated-sp-the-answer-is-no.md)

Data can prove something, as well as data can cheat some people. Gossip is fun, but one has to be seriously careful if one's gossip can ruin others' reputation. 


In one of @paulag's latest posts some data were displayed. Frankly speaking, I read some of @paulag's data analysis reports, which were impressive and useful. However, the post [Can the Data Tell us Why Ned Undelegated so much Steem Power?](https://cnsteem.com/steemit/@paulag/can-the-data-tell-us-why-ned-undelegated-so-much-steem-power-steemit-business-intelligence#@dapeng/re-paulag-can-the-data-tell-us-why-ned-undelegated-so-much-steem-power-steemit-business-intelligence-20171027t093322442z) was rather disappointing. The hints or conclusions of this post were unreliable to my comment sense. As the author said that 'the data is correct', I decided to see if it is true.


The data displayed in this post were taken from Steemsql held by @arcange.


### The Data in @paulag's Post Was Incorrect


It is easy to find that the first table in @paulag's post disagrees with the chart. The maximum of @surpassinggoolge's votes (grey area) was 700 votes per day in the chart, while the average was 1327.4  votes per day. **Apparently wrong. The average cannot be greater than the maximum.**


![](https://steemitimages.com/DQmYu6ghDtHpKWnDWZ5BboaiPeFpN3zvPvPvLfCXC6URrNR/1.png)


Image taken from @paulag's Post.



So, what is the truth?


Let's firstly see the time when @ned delegated and undelaged the SP.



| delegator | delegatee        | vesting_shares | timestamp           |
| :-------- | :--------------- | -------------: | :------------------ |
| ned       | htliao           |     1029059275 | 2017-08-08 15:15:00 |
| ned       | nicolemoker      |     1029059275 | 2017-08-08 15:15:18 |
| ned       | linuslee0216     |     1029059275 | 2017-08-08 15:15:45 |
| ned       | tumutanzi        |     1029059275 | 2017-08-08 15:16:54 |
| ned       | sweetsssj        |     1029059275 | 2017-08-08 15:20:45 |
| ned       | surpassinggoogle |     1029059275 | 2017-08-08 15:25:18 |
| ned       | ramengirl        |     1029059275 | 2017-08-08 15:28:24 |
| ned       | sweetsssj        |              0 | 2017-10-24 11:54:27 |
| ned       | ramengirl        |              0 | 2017-10-24 11:57:30 |
| ned       | nicolemoker      |              0 | 2017-10-24 11:58:57 |
| ned       | tumutanzi        |              0 | 2017-10-24 12:02:51 |
| ned       | htliao           |              0 | 2017-10-24 12:03:09 |
| ned       | linuslee0216     |              0 | 2017-10-24 12:03:21 |


If we ignore the fist day and the last day, each delegation lasted 76 days. 


```

SELECT * FROM TxVotes WHERE voter IN ('htliao',  'linuslee0216', 'nicolemoker', 'surpassinggoogle', 'sweetsssj', 'tumutanzi',  'ramengirl') AND timestamp BETWEEN '2017/08/09' and '2017/10/24

```





In  @paulag's post, nicolemoker voted 3114 times in total. 3114 / 76. How could the average votes per day be 207.6? 






I examined the data and got a new table:



| Voter            | No of Votes | Average votes per day |
| :--------------- | ----------: | --------------------: |
| nicolemoker      |        3093 |              40.69737 |
| ramengirl        |        3971 |              52.25000 |
| surpassinggoogle |       19901 |             261.85526 |
| linuslee0216     |        5555 |              73.09211 |
| htliao           |        9759 |             128.40789 |
| tumutanzi        |        7680 |             101.05263 |
| sweetsssj        |        9626 |             126.65789 |


The daily averages are around 1/5 of @paulag's calculations.


The numbers of votes are slightly different from @paulag's, perhaps because  @paulag's post took a different period of delegation, which was not mentioned in @paulag's post. This slight difference could be simply ignored.


Based on @paulag's **incorrect calculation**, all the subsequent numbers and conclusions were wrong, including the '$457K', 'Voting over 1300 times a day, this does not surprise me','...


What still makes sense is the pie chart, some ratios and percentages, and the cluster diagram. **However, I would double check them, as the post was carelessly written in  the first place.** 





### Facts or Opinions?


It seems that @paulag's post was intended to give  some facts or data, but actually it was giving only some opinions based on wrong data and groundless assumptions.


In the section 'Transfer data', @paulag's post gave three conclusions:


> 1 Reading the top memo on the table below, it very quickly because clear that @htliao was selling votes.

> 2 The data clearly shows @sweetsssj was also selling votes.


I doubt what 'selling' means here. In my mind, if A sells somehing to B, it means that B pays A money and takes something away from A. But in @paulag's data, you can only see B paid A money. What did B take away from A? If nothing, was A selling? If I transfer some SBD to @paulag, can I immediately say that  @paulag is selling votes to me?


I am sure that **the logic of @paulag' post was broken**.


> 3 Within the memo for @htliao were also suggestions that @htliao may be leasing out some power.


This conclusion was based on the transfer and delegation history between @htliao and @justyy. Many people have explained that justyy was just collecting some SP so as to support minnows. As a feedback and acknowledgement, justyy paid some so-called 'interests' to the delegators. I delegated some. Besides @htliao and me, there have been some other delegators too, receiving interests from justyy everyday. It was not surprising that @paulag's post did not mention this, because **the author knew nothing about the minnow support program.**


**As @paulag's post gave incorrect data, broken logic, and knew nothing about some facts, I think the post makes no sense to its title. Furthermore, it is badly misleading many readers, and ruining the reputations  of the innocents.**


'I also decided to have a dig through the memos,' said @paulag's post. I am looking forward to a further report, hopefully with no mistakes. This post of mine is only mentioning the mistakes in @paulag's post itself rather than my opinion to the author in person. I really like @paulag's previous reports, especially the nice charts in them. I wish @paulag could share the excel sheets so as to make the data analysis reproducible, repeatable, and reliable.


### Voting with bots?


The wrong data in @paulag's post, especially the daily average votes, e.g. voting over 1300 times a day, mislead some people. They thought that these lucky guys  voted with bots.  Is voting with bots forbidden or a shame? I do not know. But let's see if they did it.


The figures below showed some 24-hour clocks, indicating the hours when they voted. The diameters of each sector showed the percentage of the quantity of their total votes.


![unnamed-chunk-69-1.png](https://steemitimages.com/DQmUCXwNUtJz8GATLHEW4gyusoK4sQ2p8Tge6KzfDhhi6ui/unnamed-chunk-69-1.png)



There were nearly no vote in some hours of htliao, linuslee0216, nicolemoker, ramengirl and tumutanzi's clocks (humans have to sleep), while surpassinggoogle's votes covered all 24 hours. If this is the reason why @ned is still delegating SP surpassinggoogle, then why did @ned undelegate from sweetsssj, whose voting hours showed  a similar pattern?


**Can the Data Tell us Why Ned Undelegated so much Steem Power? Apparently the answer is 'no'. Data only show the facts (if the data is correct ), rather than the cause or intention. Only @ned himself can tell us the answer.**


### Before and after @ned's Delegation


What happend after @ned's delegation? See the comments (posts + replies) under cn category in the figure below. The vertical line indicates the date when @ned delegated SP.



![unnamed-chunk-70-1.png](https://steemitimages.com/DQmamLMPh6nqbnyppRMqsCVcgXBPEpq43id8UwnW7DmYUYm/unnamed-chunk-70-1.png)


Before ned's delegation, there were averagely 579 comments per day under cn category. After ned's delegation, there were averagely 1600 comments per day under cn category.


We will see what will happen after ned's undelegation. If ned's delegation was an experiment, I think his undelegation was the beginning of another.


PS. If you find any mistakes in my post, please let me know and you are highly appreciated.


---


本文是对污蔑几位临时大鲸的帖子 [Can the Data Tell us Why Ned Undelegated so much Steem Power?](https://cnsteem.com/steemit/@paulag/can-the-data-tell-us-why-ned-undelegated-so-much-steem-power-steemit-business-intelligence#@dapeng/re-paulag-can-the-data-tell-us-why-ned-undelegated-so-much-steem-power-steemit-business-intelligence-20171027t093322442z) 的反驳。中文翻译过来就是：污蔑帖子用的数据是错的，计算是错的，逻辑是错的，而且不了解一些基本事实，所以纯属胡说八道。谢谢。
