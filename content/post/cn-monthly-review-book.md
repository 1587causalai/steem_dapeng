---
title: "\"月旦评文集\"征求大家的意见"
author: dapeng
date: "2017-09-21 09:21:54"
slug: cn-monthly-review-book
categories: [cn]
tags: 
  - cn
  - cn-reader
  - cran
  - steemswatch
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/cn-monthly-review-book), [cnsteem](https://cnsteem.com/cn/@dapeng/cn-monthly-review-book), [chainbb](https://chainbb.com/cn/@dapeng/cn-monthly-review-book), [busy](https://busy.org/cn/@dapeng/cn-monthly-review-book), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/cn-monthly-review-book.md)

大家翘首以盼的“[月旦评](https://steemit.com/cn/@rivalhw/3pugju)”活动，终于轰轰烈烈地拉开了序幕。看看组委会名单，阵容豪华得晃眼睛，我都不敢直视……赶紧低下头，该干啥干啥。


一低头，就看到 @lemooljiang 做出了[最高指示](https://steemit.com/cn/@rivalhw/6apkrp-steemit#@lemooljiang/re-rivalhw-re-lemooljiang-re-rivalhw-6apkrp-steemit-20170916t104939604z)：


> 最好看下能不能做成文集保存下来，也算是大家的一点小成果！


这任务我接了，谁都别拦我，拦也拦不住。不久前，我刚刚[为谷哥点名做了一次文集](https://steemit.com/cn/@dapeng/6wpnvk)。“月旦评文集”的任务简直就是为我量身定做的。


---


先给大家看一下“月旦评”文集的预期效果吧，下面是我自己文集其中两个，作为示例。


第一个范例是我的中文育儿博客合集《[爸爸三定律](https://bookdown.org/baydap/papasdiary/three-laws.html)》。发布在网上的模样是这样的：


![bookdown1.jpg](https://steemitimages.com/DQmP5XxTH4GmZ4XzYirEbWGk6RvyyLi4KE2B3LvaahtC7re/bookdown1.jpg)



pdf 格式文档是这样的（点击图片看大图：封面，目录，正文）：


[![Slide1.JPG](https://steemitimages.com/DQmW8XrM5SnTcY7gbzeUigfkAzoZC7PGyTw4aLmphn4ZZLo/Slide1.JPG)](https://steemitimages.com/DQmW8XrM5SnTcY7gbzeUigfkAzoZC7PGyTw4aLmphn4ZZLo/Slide1.JPG)


第二个范例是我写的一本英文书 [R bookdownplus Textbook](https://bookdown.org/baydap/bookdownplus/)。发布在网上的模样是这样的：


![bookdown2.jpg](https://steemitimages.com/DQmNRShVSAAk78RsXR6uPiHLNNnar65ozjjnEiBy43nvKE5/bookdown2.jpg)


pdf 格式文档是这样的（点击图片看大图：封面，目录，正文）：


[![Slide2.JPG](https://steemitimages.com/DQmfX7uhByRt9ZRNUBmxKWBGyQjNycxcPw1qzddJpg1JzVX/Slide2.JPG)](https://steemitimages.com/DQmfX7uhByRt9ZRNUBmxKWBGyQjNycxcPw1qzddJpg1JzVX/Slide2.JPG)


我的初步设想是：


- “月旦评文集”可以每期一册，每年可以做一本合订本，或精选集。

- 每册文集都有个固定网址。打开网址，就看到上面展示的网页版。

- 网页上方的几个按钮，分别是显示目录、搜索、改变字体、修改（**是的，文集永远可以修改！脱离了区块链的限制！**）、下载、分享等。下载按钮按下去，就可以下载文集的其他格式，包括 epub（下载到手机上离线阅读），pdf（精致排版方便打印）和 word 文档。


---


下面简单说说这是怎么做出来的。对技术不感兴趣的请跳过，直接读文末最后一部分。


熟悉我的人都知道，我是 R 语言的粉丝。以前写的“大鹏观察”系列帖子，数据的获取、分析、作图，甚至 markdown 文件的编写，用的都是 R 语言。


R 语言的 bookdown 程序包，天生就是为了把 markdown 文件做成文集。而steemit 的源文件，就是 markdown。


steemit 想做文集而遇到 bookdown，简直是孙悟空遇到定海神针：史上最称手兵器，前世量身打造！


可惜的是，原生的 bookdown 用起来不是那么方便。所以，前不久，我开发了个 R 程序包，叫做 bookdownplus，已经[在 CRAN 正式发布](https://CRAN.R-project.org/package=bookdownplus)，相当于 bookdown 的咖啡伴侣。


所以，上面的文集范例，都是用我自产自销的 bookdownplus 做出来的。


---


方案是现成的，稍作修改就能用。但是，显然我们不会止步于“能用”。我们要做得更好。


首先，**为了减少文集里的格式混乱和错误，建议大家在投稿里注意**：


- 插图时请使用 markdown 语法，不要用 html 语法。这是为了方便制作 pdf。

- 不要滥用标题格式。有些帖子为了强调正文里某些???字，就用标题格式`#`，这是不合规矩的。正文就是正文，只有标题才适合用标题格式。想强调的话，用**粗体**`**粗体**`足矣。

- 对 markdown 不熟的话，建议使用 Typora 编辑器，详见[我写的教程](https://steemit.com/cn/@dapeng/markdown-steemit-tips-the-best-markdown-editors)。


当然，这是建议，不是强求。如果你不按这个建议，只是最后增加了制作文集的工作量，增加了文集里的错误格式而已。格式太混乱的话，可能最后被踢出文集……


此外，我想征求大家的意见和帮助。例如:


- 有没有哪位可以设计个封面，作为pdf 文档的首页？“月旦评”文集可以每期换一个封面，也可以不换。大家说呢？

-  R 语言可以方便地往文集里插入“大鹏观察”的统计数据，例如在文集后面加个附录，列出关键词词云图、参赛选手的声望值分布、年龄分布等等。大家说说需要什么数据，我就加什么数据。


大家还有别的什么建议？欢迎在这里留言。


![end.png](https://steemitimages.com/DQmb3NCyeZRFcGHDKGXW1i3K23gwFY1xwva7LqG7wpCqKCb/end.png)
