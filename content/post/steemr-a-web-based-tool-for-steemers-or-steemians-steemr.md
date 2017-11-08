---
title: "steemr: an easy web-based tool for Steemians 开发了一个易用的在线小工具 steemr"
author: dapeng
date: "2017-07-27 13:23:39"
slug: steemr-a-web-based-tool-for-steemers-or-steemians-steemr
categories: [cn]
tags: 
  - cn
  - steem
  - steemit
  - cn-programming
  - steem-tools
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/steemr-a-web-based-tool-for-steemers-or-steemians-steemr), [cnsteem](https://cnsteem.com/cn/@dapeng/steemr-a-web-based-tool-for-steemers-or-steemians-steemr), [chainbb](https://chainbb.com/cn/@dapeng/steemr-a-web-based-tool-for-steemers-or-steemians-steemr), [busy](https://busy.org/cn/@dapeng/steemr-a-web-based-tool-for-steemers-or-steemians-steemr), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/steemr-a-web-based-tool-for-steemers-or-steemians-steemr.md)

In my previous post [*New Steemians, have you ever thought about your data privacy? (1)*](https://steemit.com/steemit/@dapeng/new-steemians-have-you-have-thought-about-your-data-privacy) , some friends asked me to make such a report for them. It might be useful to develop an on-line tool for every Steemer/Steemian. Thus I have developed [steemr](http://steemr.org).


It is easy to use. Click the `Follower report`  tab and input an ID , or click the `Voter report`  tab and input the link of post you are interested in. Then click `GO`. Wait 5 -- 20 seconds and you will see the results.


It is only a tip of the iceberg. More features of this tool are coming soon. 


Think twice before blogging on Steemit. You can't put the genie back in the bottle,  and  it is no use crying over spilt milk.


![steemr-fr.jpg](https://steemitimages.com/DQmcdcBY7j8ntos4qcu1HVsUYTd2WgCPH8SfwHTnDqdJG4J/steemr-fr.jpg)


![steemr-vr.jpg](https://steemitimages.com/DQmS9hzu1w1wkqeruLwxR1X2FUtekL6mHdUxJvmBkrhFiDZ/steemr-vr.jpg)


在[Steemit 的新手们，你们考虑过数据隐私的问题吗 (1)](https://steemit.com/steemit/@dapeng/new-steemians-have-you-have-thought-about-your-data-privacy) 一文发布后，的确有朋友要我对他的 ID 的关注者信息也写一个类似的报告。我想，不如开发个在线工具，大家谁想查就自己查吧。于是就有了 [steemr](https://pzhao.shinyapps.io/steemr/)。


用起来很简单：


- 点击 `Follower report` 标签，输入你想查的 ID，点击 `GO` 按钮，等几秒钟或十几秒钟（取决于服务器的速度和 你要查的 ID 的情况）就可以看到结果了，包括粉丝 （followers） ID 的词云图，按这些粉丝的粉丝数量、发帖数量和vests大小??序。如果粉丝超过30个，就取前三十个。词云图下方，还给出了尚未互粉的 ID 列表。

-  点击`Voter report`  标签，输入你想查的帖子链接（可以是完整链接，也可以是从@符号开头到末尾），点击 `GO` 按钮，等几秒钟或十几秒钟，就可以看到为该帖点赞的名单和百分比。图下面给出了尚未投票的粉丝名单（类似的工具有 [ @justyy 的网页界面](https://helloacm.com/tools/steemit/who-has-not-voted/ ) ，[ @beautifulbella 的Excel 方法](https://steemit.com/cn/@beautifulbella/use-excel-to-find-your-friends-who-does-not-upvote-you-excel)，[ @oflyhigh 的Python 方法](https://steemit.com/cn/@oflyhigh/voter-list)）。


本工具以后会进一步开发完善。这只是冰山的一角。再次提醒大家：在 steemit 发文发照片要三思，免得后悔，覆水难收。
