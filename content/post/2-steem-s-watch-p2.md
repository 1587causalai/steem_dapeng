---
title: "谷哥点名第 2 期“第一次”回顾（大鹏观察 Steem's Watch P2）"
author: dapeng
date: "2017-08-27 20:45:54"
slug: 2-steem-s-watch-p2
categories: [cn]
tags: 
  - cn
  - cn-programming
  - steemit
  - steemit-stats
  - steemswatch
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/2-steem-s-watch-p2), [cnsteem](https://cnsteem.com/cn/@dapeng/2-steem-s-watch-p2), [chainbb](https://chainbb.com/cn/@dapeng/2-steem-s-watch-p2), [busy](https://busy.org/cn/@dapeng/2-steem-s-watch-p2), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/2-steem-s-watch-p2.md)

“[谷哥点名](https://steemit.com/cn/@jubi/42wvdr)”是 steem 中文社区 @jubi 发起的半命题作文活动。“大鹏观察”旨在对参赛帖子进行一些数据分析和挖掘，展示一些有趣的结果，希望对以后的活动具有一些参考价值。使用的数据来源是 steemdata.com，数据获取、分析、图表制作、报告编写全程使用人见人爱的 R 语言。仅供参考，如果有数字与官方有出入，请以官方为准。


大鹏观察： 谷哥点名第2期回顾

----------------------------


### 参赛基本信息


-   主题：第一次

-   日期：2017-08-09 -- 2017-08-16

-   发起：[“谷哥点名”第2期开始](https://steemit.com/cn/@jubi/4tsdsb-and)

-   颁奖：[“谷哥点名”第2期结束](https://steemit.com/cn/@jubi/sxzgw-and)

-   参赛作品列表：见文末。


### 帖中之最


本期活动参赛作品共 65 篇。获奖作品的介绍已经在本文开头给出了链接，是按 google 搜索结果排名的，不再赘述。我们也可以用其他方式排名，来看看参赛作品里几个第一名。


**字符最多**


-   [第一次 - 在第一次家族旅行 - 台中 (內有家族旅行的心得）| The first time - My first family trip - Tai Chung](https://steemit.com/@carinewhy/or-the-first-time-my-first-family-trip-tai-chung)，含 9500 个字符。


**插图最多**


-   [第一次 - 在第一次家族旅行 - 台中 (內有家族旅行的心得）| The first time - My first family trip - Tai Chung](https://steemit.com/@carinewhy/or-the-first-time-my-first-family-trip-tai-chung)，含 51 张图片。


**修改间隔最长**


-   [Original poetry 第一次绝恋--最后的初恋 The first but also last love.](https://steemit.com/@tvb/the-first-but-also-last-love)，??布 139.3 小时即 5.8 天之后，作者做了最后一次修改。


**得赞最多**


-   [第一次使用STEEMSQL查询谷哥点名数据](https://steemit.com/@oflyhigh/steemsql)，得到 330 个赞。


**赚钱最多**


-   [第一次使用STEEMSQL查询谷哥点名数据](https://steemit.com/@oflyhigh/steemsql)，收入为 243 美元。


**帖子正文里出现最多的关键词**


下面是所有帖子里出现的字符长度超过 2 个、出现次数超过 10 次的中文关键词词云图。字符越大，在全部帖子里重复出现的次数就越多。当然，我们去掉了本期指定的关键词"第一次"。


![unnamed-chunk-7-1.png](https://steemitimages.com/DQmPabXLoBUzSsbUpRq7HYFKGWrHwcgeEHt7zVFMWS5Zgar/unnamed-chunk-7-1.png)


### 参赛选手


下图是参赛选手的注册 ID 序号分布图。全网目前共有 325451 个 ID。参赛选手中一半以上都排在第 209970 个注册 ID 之后。排在最前面的是第 18783 个 ID，最后面的是 第 307645 个 ID。猜猜他们都是谁？


![unnamed-chunk-8-1.png](https://steemitimages.com/DQmPs7wH93zSzCcZUgv6p65zVHCdugUjqzzRWi3EW2t6xy6/unnamed-chunk-8-1.png)


下图是参赛选手的注册日期分布图。大部分参赛者都是 2017 年 5 月后注册的新朋友，尤其是 2017 年 7 月注册的居多。也有一些早期用户。


![unnamed-chunk-9-1.png](https://steemitimages.com/DQmYpcCHHAz3iq1ECCgnVi7yT4TZhDoCAhXYkDaiwLDaBNX/unnamed-chunk-9-1.png)


### 发帖


活动期间，每天累计发帖总数：


![unnamed-chunk-10-1.png](https://steemitimages.com/DQmS5nz9eDxZL2KUWsSRTJzw9oThdLC29whQDHiWA7pygQk/unnamed-chunk-10-1.png)


下图是个特殊的时钟，一圈是24小时，显示了一天24小时里发帖的频次，面积越大的时段，发帖数就越多。红线显示的是频次分布：每两条相邻红线之间的帖子数，占全部帖子数的 25%。哪两条红线最接近，哪两条红线之间就是发帖高峰时段。


可以发现，在标准时间 5 点到 9 ???发帖的人最多。


![unnamed-chunk-11-1.png](https://steemitimages.com/DQmdrWQmDNYiF2pkVZZe2qHv8iUPriFouf9zqDZcxCrW8xJ/unnamed-chunk-11-1.png)


本活动是在 'cn' 板块发起的，参加活动的帖子自然都贴上了该标签以及子区标签。我们看看除此之外，大家还使用了那些标签以及使用频率。


![unnamed-chunk-12-1.png](https://steemitimages.com/DQmQZ7Heh9fTJJRxVSXvYyHjNbUf5hUL98vvX8ke34Mfwxd/unnamed-chunk-12-1.png)


### 收入


最后我们来谈钱。下图显示的是单篇帖子收入的分布。横坐标是美元，阴影面积越大，对应美元的帖子数量越多。 参与活动的 65 篇帖子，总收入为 2295.02 SBD， 单帖收入最高为 243.24 SBD，平均每帖收入为 35.31 SBD。


![unnamed-chunk-13-1.png](https://steemitimages.com/DQmevt3HaRUbhxPD2GDjWxY4CJMFZ6UkasFkkCZE3LvaSqn/unnamed-chunk-13-1.png)


下图是各篇帖子获得的投票（点赞）数。 累计得赞 2972 个，单帖得到的点赞数最高为 330 个，平均每帖得赞 45.7 个。


![unnamed-chunk-14-1.png](https://steemitimages.com/DQmY6455yyZ4z3CQFGzSMuzWZUTr1qXgJNQdcvYDJyaUYNB/unnamed-chunk-14-1.png)


为本次活动能够投票次数最多的前三位是 @jubi, @linuslee0216, @htliao。下面是投票次数超过 10 次的 ID 词云图。


![unnamed-chunk-15-1.png](https://steemitimages.com/DQmRD2Xjk86zB8bNEK1VSeSwsTfM2VvRsGXyYU37QZ4xVQA/unnamed-chunk-15-1.png)


为本次活动点赞收入贡献最多的前三位伯乐是 @abit, @linuslee0216, @tumutanzi。他们一共贡献了全部收入的 60%。排在他们后面的第 4 到第 10 位的贡献比例如下图。感谢他们的支持！


![unnamed-chunk-16-1.png](https://steemitimages.com/DQmdZy31DtfJYcAqbLYxbYfECe3zEKbrxW9HWagSHF266FK/unnamed-chunk-16-1.png)


------------------------------------------------------------------------


感谢关注“大鹏观察”。欢迎关注和参加下一期的活动，也欢迎提出宝贵意见。谢谢。


### 附录：参赛作品列表


| created             | author            | title                                    |
| :------------------ | :---------------- | :--------------------------------------- |
| 2017-08-09 07:10:30 | @pakyeechan       | [第一次 - 離鄉別井 - “谷哥点名”活动](https://steemit.com/@pakyeechan/or) |
| 2017-08-09 08:31:15 | @dixonloveart     | [相约大美新疆,第一次在第13届全国冬运会现场 Meet the beauty of Xinjiang,first time in China national winter games](https://steemit.com/@dixonloveart/13-meet-the-beauty-of-xinjiang-first-time-in-china-national-winter-games) |
| 2017-08-09 10:15:33 | @mrspointm        | [My first encounter with steemit/我与steemit的第一次邂逅 - 谷歌点名](https://steemit.com/@mrspointm/my-first-encounter-with-steemit-steemit-or) |
| 2017-08-09 10:31:48 | @sunnyjolly       | [我人生的N种第一次](https://steemit.com/@sunnyjolly/n) |
| 2017-08-09 10:52:12 | @icedream         | [第一次认识这个世界](https://steemit.com/@icedream/2rutwi) |
| 2017-08-09 11:00:00 | @livinguktaiwan   | [第一次 - 英國行山篇 "谷歌点名"活動 Hiking South Downs Way England](https://steemit.com/@livinguktaiwan/59nvof) |
| 2017-08-09 13:07:39 | @xiaolizi         | [【参加谷哥点名】我在Steemit的第一次发帖](https://steemit.com/@xiaolizi/steemit) |
| 2017-08-09 14:12:33 | @herlife          | [第一次离开熟悉的地方外出闯荡](https://steemit.com/@herlife/3y1gfc) |
| 2017-08-09 14:26:54 | @kitcat           | [成就人生的第一次](https://steemit.com/@kitcat/3bfjat) |
| 2017-08-09 17:11:42 | @zhijun           | [第一次 // First Time](https://steemit.com/@zhijun/first-time) |
| 2017-08-09 18:12:18 | @candiceji        | [人生第一次——不仅有酸甜苦辣，更有悲欢离合](https://steemit.com/@candiceji/7dq4r7) |
| 2017-08-10 00:34:03 | @ace108           | [第一次 - The First Time (Chinese content only but feel free to comment in English if you understsand) - (by @ace108)](<https://steemit.com/@ace108/chinese-content-only-but-feel-free-to-comment-in-english-if-you-understsand-by-ace108>) |
| 2017-08-10 01:11:24 | @aaronli          | [第一次， 细看妈妈的皱纹- “谷哥点名”活动](https://steemit.com/@aaronli/or) |
| 2017-08-10 01:22:15 | @superhardness    | [爱上第一次--First Exploration](https://steemit.com/@superhardness/first-exploration) |
| 2017-08-10 01:24:48 | @victorier        | [如何看待你人生中的第一次？](https://steemit.com/@victorier/2vxpy6) |
| 2017-08-10 02:06:03 | @laodr            | [老道茶館 －請上坐，喝杯茶，說點事；今日話題－第一次 （跨域合作：茶館Ｘ谷哥点名）](https://steemit.com/@laodr/laodr-tea-house-170810) |
| 2017-08-10 03:55:33 | @yinlovesu0914    | [\#隨筆2 第一次 - 谷哥点名](https://steemit.com/@yinlovesu0914/2) |
| 2017-08-10 04:09:12 | @coldhair         | [第一次在星级大酒店吃饭](https://steemit.com/@coldhair/3dqe3s) |
| 2017-08-10 04:37:30 | @tvb              | [Original poetry 第一次绝恋--最后的初恋 The first but also last love.](https://steemit.com/@tvb/the-first-but-also-last-love) |
| 2017-08-10 05:10:51 | @hannahwu         | [第一次品味人生百态 My First Time - Ups and Downs in Life](https://steemit.com/@hannahwu/my-first-time-ups-and-downs-in-life) |
| 2017-08-10 05:14:57 | @shirlam          | [第一次 ── 我和我的友生](https://steemit.com/@shirlam/4grndt) |
| 2017-08-10 05:44:24 | @herlife          | [第一次拿到在steemit上写作的钱](https://steemit.com/@herlife/steemit) |
| 2017-08-10 06:52:42 | @sylvia1997       | [领导，今天是我第一次喝酒，可不可以。。。](https://steemit.com/@sylvia1997/4ctrkh) |
| 2017-08-10 11:40:54 | @blacktranquility | [第一次去博物馆之中国古代的酒具 The ancient wine cups of the Chinese history](https://steemit.com/@blacktranquility/the-ancient-wine-cups-of-the-chinese-history) |
| 2017-08-10 13:56:00 | @cornelia         | [第一次去油菜花地里玩，种下了心灵里的树](https://steemit.com/@cornelia/6fjigk) |
| 2017-08-10 18:45:03 | @kenchung         | [My first and long leave from my hometown // 第一次離鄉別井](https://steemit.com/@kenchung/my-first-and-long-leave-from-my-hometown) |
| 2017-08-10 21:50:18 | @bxt              | [The first time i made my rose steamed buns 第一次做玫瑰花馒头！](https://steemit.com/@bxt/the-first-time-i-made-my-rose-steamed-buns) |
| 2017-08-10 23:03:06 | @linuslee0216     | [第一次 — 住在大学宿舍经历 / 谷哥点名活动 - My university life, my first time living in a university hostel](https://steemit.com/@linuslee0216/or-my-university-life-my-first-time-living-in-a-university-hostel) |
| 2017-08-11 01:16:42 | @carinewhy        | [第一次 - 在第一次家族旅行 - 台中 (內有家族旅行的心得）- The first time - My first family trip - Tai Chung](https://steemit.com/@carinewhy/or-the-first-time-my-first-family-trip-tai-chung) |
| 2017-08-11 01:30:00 | @guyverckw        | [很多第一次的第一次 - "谷哥点名"](https://steemit.com/@guyverckw/or) |
| 2017-08-11 04:10:27 | @mrpointp         | [第一次“体验”做父母的感觉 / The First Time for Being a "Parent" - 谷歌点名](https://steemit.com/@mrpointp/the-first-time-for-being-a-parent) |
| 2017-08-11 06:23:21 | @incrediblesnow   | [第一次来华文区时的情景与华文区如何发展](https://steemit.com/@incrediblesnow/79hzy9) |
| 2017-08-11 08:18:54 | @bestmz           | [第一次注册域名](https://steemit.com/@bestmz/ftczm) |
| 2017-08-11 09:15:57 | @biuiam           | [第一次，科學研究的第一次/ “谷哥点名”活动 The First time: The Tirst Time for Scientific Research](https://steemit.com/@biuiam/the-first-time-the-tirst-time-for-scientific-research) |
| 2017-08-11 09:28:42 | @hopsken          | [第一次去海边 —— “温良恭俭让”的北威尔士海滨小镇兰迪德诺](https://steemit.com/@hopsken/35ffg5) |
| 2017-08-11 09:36:03 | @krischy          | [第二期“谷哥点名”???動： 第一次 離鄉別井](https://steemit.com/@krischy/6jpatl) |
| 2017-08-11 10:22:18 | @wilkinshui       | [我的第一次的虛擬人生](https://steemit.com/@wilkinshui/4xkxlc) |
| 2017-08-11 10:37:51 | @rencircle        | [一天之内的两个第一次](https://steemit.com/@rencircle/3ewrb2) |
| 2017-08-11 12:05:33 | @oflyhigh         | [第一次使用STEEMSQL查询谷哥点名数据](https://steemit.com/@oflyhigh/steemsql) |
| 2017-08-11 14:28:15 | @blacktranquility | [历史的传承~第一次去博物馆](https://steemit.com/@blacktranquility/5sorag) |
| 2017-08-11 14:39:03 | @chaofanjun       | [我第一次挑大梁就让公司损失了20万](https://steemit.com/@chaofanjun/20) |
| 2017-08-11 15:30:33 | @jessicameng      | [第一次危险那么近 （分享：留学时的真实经历）](https://steemit.com/@jessicameng/32tqsx) |
| 2017-08-11 17:34:45 | @tiffchiuhk123    | [第一次戀愛](https://steemit.com/@tiffchiuhk123/7lqic) |
| 2017-08-11 22:36:15 | @magicmonk        | [第一次 打網球 Playing tennis for the first time](https://steemit.com/@magicmonk/playing-tennis-for-the-first-time) |
| 2017-08-12 00:33:18 | @fundurian        | ["谷哥点名", 我的第一次倒霉事](https://steemit.com/@fundurian/4jgfas) |
| 2017-08-12 01:42:42 | @syh7758520       | [第一次距离死亡那么近------谷哥点名二期](https://steemit.com/@syh7758520/79qx58) |
| 2017-08-12 02:45:39 | @wseemfree        | [第一次使用blocktrades](https://steemit.com/@wseemfree/blocktrades) |
| 2017-08-12 03:40:03 | @leogor1234       | [第一次踏進公開試的試場 - 谷歌點名第二期](https://steemit.com/@leogor1234/2aqqc) |
| 2017-08-12 04:19:15 | @timknip          | [第一次连写三篇恐怖小说，原来可以这么短](https://steemit.com/@timknip/5zhfhd) |
| 2017-08-12 05:11:24 | @doggieandfoodie  | [Throwback- The First Day We Met 第一次見面](https://steemit.com/@doggieandfoodie/throwback-the-first-day-we-met) |
| 2017-08-12 08:12:45 | @zsilence         | [[谷哥点名]第一次被骗的经历](https://steemit.com/@zsilence/muuvv) |
| 2017-08-12 09:06:45 | @richen           | [男生也要保養?! 第一次護臉](https://steemit.com/@richen/3l95fj) |
| 2017-08-12 10:46:48 | @flyingcondor     | [第一次 - 我全新生活的体会](https://steemit.com/@flyingcondor/eqhbe) |
| 2017-08-12 20:15:12 | @plokmi           | [第一次](https://steemit.com/@plokmi/2nlzp8) |
| 2017-08-13 03:09:51 | @lydiachan        | [第一次, 上洗手間遇到史無前例的窘境!!! 冏](https://steemit.com/@lydiachan/5pyxz9) |
| 2017-08-13 13:08:45 | @nigulax          | [谷歌点名第二期: 第一次](https://steemit.com/@nigulax/5wwpfu) |
| 2017-08-13 21:50:18 | @dapeng           | [第一次将“谷哥点名”活动整理成文集](https://steemit.com/@dapeng/6wpnvk) |
| 2017-08-14 07:13:27 | @luneknight       | [第一次陪床](https://steemit.com/@luneknight/2ryxd2) |
| 2017-08-14 08:01:12 | @blacktranquility | [谷歌点名 '第一次' 目前的排名情况](https://steemit.com/@blacktranquility/6x3uzs) |
| 2017-08-14 11:43:12 | @justyy           | [第一次打肿脸充胖子 - 花了200STEEM租1万SP四周！](https://steemit.com/@justyy/200steem-1-sp) |
| 2017-08-14 14:08:33 | @gladysmak        | [Day Off in Hong Kong : My First Time Standup Paddleboarding in Big Wave Bay,Shek O / 我在香港的第一次立槳衝浪經驗 (Eng/中文）](https://steemit.com/@gladysmak/day-off-in-hong-kong-my-first-time-standup-paddleboarding-in-big-wave-bay-shek-o-eng) |
| 2017-08-14 16:17:33 | @lonsoft          | [第一次远行](https://steemit.com/@lonsoft/6sjkod) |
| 2017-08-14 17:04:33 | @jiangchen        | [无数的第一次，只是为了每一次的精彩](https://steemit.com/@jiangchen/4d3k1k) |
| 2017-08-15 05:17:54 | @xyj              | [Drawing Challenge\#2 画荷花 第一次参加画画挑战](https://steemit.com/@xyj/zewc7) |
| 2017-08-15 23:57:39 | @mcw              | [第一次，進入研究實驗室的第一次/ “谷哥点名”活动 The First time: The First Time enter a research lab](https://steemit.com/@mcw/the-first-time-the-first-time-enter-a-research-lab) |


------------------------------------------------------------------------



tags: #cn-programming #steemit #steemit-stats #steemswatch
