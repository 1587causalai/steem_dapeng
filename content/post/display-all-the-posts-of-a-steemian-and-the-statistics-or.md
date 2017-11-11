---
title: "Steemr: Display all the posts of a steemian and the statistics - 展示一个账户的所有帖子和统计数据"
author: dapeng
date: "2017-11-09 22:39:33"
slug: display-all-the-posts-of-a-steemian-and-the-statistics-or
categories: [steemdev]
tags: 
  - steemdev
  - steemit
  - cn
  - programming
  - steemdata
---

原文链接: [steemit](https://steemit.com/steemdev/@dapeng/display-all-the-posts-of-a-steemian-and-the-statistics-or), [cnsteem](https://cnsteem.com/steemdev/@dapeng/display-all-the-posts-of-a-steemian-and-the-statistics-or), [busy](https://busy.org/steemdev/@dapeng/display-all-the-posts-of-a-steemian-and-the-statistics-or), [chainbb](https://chainbb.com/steemdev/@dapeng/display-all-the-posts-of-a-steemian-and-the-statistics-or), [steemdb](https://steemdb.com/steemdev/@dapeng/display-all-the-posts-of-a-steemian-and-the-statistics-or), [steemd](https://steemd.com/steemdev/@dapeng/display-all-the-posts-of-a-steemian-and-the-statistics-or), [busy](https://busy.org/steemdev/@dapeng/display-all-the-posts-of-a-steemian-and-the-statistics-or), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_dapeng/master/content/post/display-all-the-posts-of-a-steemian-and-the-statistics-or.md)

It is hard to see all the posts of a steemian on steemit. You have to scroll down your browser, wait, and scroll, and wait ...... Nothing is more boring if the author has hundreds of posts and you want to see the oldest one, which might be the self-introduction post.  

I was suffering this problem for a long time. Today I could not stand it any longer. Thus I developed a web app: http://steemr.org.

Input an ID and press Enter, you can see a table of all the posts. Features:

- The table displays 20 posts per page by default. You could change the number on the top-left of the table to display 50 or 100 posts per page, or all the posts.

- The time, payout and vote number are given. Click the column name and you can sort the posts.

- Type something as keywords in the top-right bar or the bottom bars, and you can filter the titles, posting time, categories and tags. For instance, type '2017-07' in the bottom date bar, and you will see only the posts posted in July 2017. See the moving picture below.  Combining the sorting feature, you can easily find the highest payout post in a given month.

- One single click (if blocked, press ctrl+click) can jump to the webpage of a post on steemit, cnsteem, chainbb, busy, steemdb, or steemd.

- Statistic diagrams show the cumulative payout, votes and post number. A 24-hour diagram shows the active hour of the author.

The following figure is an example, showing the growth of the cumulative payout of @deanliu's posts.

![payout.png](https://steemitimages.com/DQmaB6PqmCqJPQNaXYPjbcsaGV7QQjcMB9VdwkTVCrg4sV6/payout.png)

Have fun!

Steem 有个让人无比郁闷的毛病：想一目了然地看一个人的所有帖子，你得往下拉，等着载入，再拉，再等......尤其是那些发布了几百上千篇帖子的大神，想看他们的旧帖，在 steemit 上难比登天。我只能去 chainbb，那里支持分页，点第一页就行了。但是，你还得点页码，仍然不是很方便。

为啥就没个文章全部列表呢？连杀人鲸 @deanliu  都[抱怨](https://cnsteem.com/cn/@deanliu/juan)：

> 我其實等待這樣的我所有文章列表很久了，Steemit老是把resteem跟自己文章放一起，大半年了，說過的人甚至走一半了，也沒見有人理會。這樣列表的好處是，可以很快找到自己的很久以前舊文章......

如今，能做到展示全部文章列表的，大概只有我量身定做的 [steem 镜像网站](https://cnsteem.com/cn/@dapeng/or-10-sbd-to-build-a-mirror-site-for-your-own-steem-posts)了（[@deanliu 的镜像](https://deancrypto.netlify.com)， [@dapeng 的镜像](https://dapeng.netlify.com/)， [@pzhao 的镜像](https://pz.netlify.com/)）。只是我仍不满意：没做镜像的怎么看？想看某人收益最高的帖子怎么办？每次都查数据库，太烦了。

于是我二话没说，操起 R 语言，光光光光，做好了，欢迎大家来调戏，地址是 http://steemr.org。是的，就是我开发的 [steem 水浒英雄榜](https://cnsteem.com/cn/@dapeng/steemit-cn)那个地址。英雄榜退居二线，给帖子一览表让让位。

![steemr20171109.gif](https://steemitimages.com/DQmZ16mP1YE9JSbNcA86aUCw82kCWssNJ1EEQohXaKt72LR/steemr20171109.gif)


只要输入个 steem 账号，按回车，就显示这个账号的所有 blog 帖子（不包含 resteemed）。功能如下：

- 默认每页显示 20 篇文章。你可以点击表格左上角的数字，选择每页 50 篇，或 100 篇，或全部显示。

- 每篇文章都给出了发布时间、收益（SBD）和点赞数量。点击标题栏，就可以实现排序。按时间顺序、逆序，按收益最大或最小，随便你排。

- 表格左上角和下方都有???索栏，可以搜索标题里的关键字。例如在 Date 一列下面的搜索栏搜索 '2017-07'，就会过滤出 2017 年 7 月的文章列表。此时再点击标题栏的 payout 排序，就筛选出 2017 年 7 月 收益最高的帖子了。

- 每篇文章都给出了在 steemit , cnsteem, chainbb, busy, steemdb, steemd 的链接，点一下直达（如果被浏览器阻挡的话，按 ctrl + 点一下就在新标签打开了）。

- 附带给出了统计图表，展示作者累计收益、累计点赞、累计文章数量和 24 小时活跃时间的统计图。

下图是 @deanliu 的作息时间图：


![24.png](https://steemitimages.com/DQmfAd47vrT4ZjMhZCKtWKj5ZcQhdagdrhPNAXKDeDn1k8G/24.png)
这个 app 我一直想做，拖拖拖拖拖到了今天才终于做出来。近期的心愿已了，我打算享受一段没有 steem 的时光，正如 @deanliu [所说](https://deancrypto.netlify.com/post/owo-farewell/)：

> 接下来这一周我将不再发文章、不再参与讨论，也不再点赞，要把时间留给这个月来被我疏忽的家庭、进度落后的工作、脸书上的朋友，以及最重要的身体的健康。毕竟，日子还长呢，养精蓄锐之后，才能为自己的SteemLife注入新的能量。

朋友们再见！下周的这个时候，我会回来给“华语好声音”颁奖。
