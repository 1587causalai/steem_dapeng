---
title: "Bug Hunting: the reward selection menu - 乌托邦的一个 bug"
author: dapeng
date: "2017-12-22 10:12:39"
slug: bug-hunting-the-reward-selection-menu
categories: [utopian-io]
tags: 
  - utopian-io
  - cn
---

原文链接: [steemit](https://steemit.com/utopian-io/@dapeng/bug-hunting-the-reward-selection-menu), [cnsteem](https://cnsteem.com/utopian-io/@dapeng/bug-hunting-the-reward-selection-menu), [busy](https://busy.org/utopian-io/@dapeng/bug-hunting-the-reward-selection-menu), [chainbb](https://chainbb.com/utopian-io/@dapeng/bug-hunting-the-reward-selection-menu), [steemdb](https://steemdb.com/utopian-io/@dapeng/bug-hunting-the-reward-selection-menu), [steemd](https://steemd.com/utopian-io/@dapeng/bug-hunting-the-reward-selection-menu), [busy](https://busy.org/utopian-io/@dapeng/bug-hunting-the-reward-selection-menu), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_dapeng/master/content/post/bug-hunting-the-reward-selection-menu.md)

### The bug: the reward selection menu is on top of the webpage

When posting a new article on Utopian.io, I can choose the reward as "100 Steem Power" or "50% SBD and 50% SP". However, when I click the choice button, these two options appear in a selection menu on top of the webpage, far away from the choice button.

Well, I am not professional on webpage development, thus I am probably using the wrong term to describe the webpage elements. Please see the screenshot as follows.

![_utopian_bug.jpg](https://res.cloudinary.com/hpiynhbhq/image/upload/v1513937203/m7cdaavcr39httdlzuxv.jpg)


I guess it is a bug. If it is intended to be on top of the webpage, it is far enough from the selection button. I used a small size of the web browser just for a better sceenshot. If I use the full sceen view of the web browser, then the choice menu is too far away to find, which is very confusing to new users. Shouldn't the options of "100 Steem Power" and "50% SBD and 50% SP" appear close to the button, like steemit as follows?

![utopian_bug.jpg](https://res.cloudinary.com/hpiynhbhq/image/upload/v1513937221/einnq07mrimlfpl8yyoj.jpg)


### My session information

I tested it on both windows 7 + Firefox 56.0 (32-bit), and Ubuntu 16.04 + Firefox 57.0.1 (64-bit).

### How to reproduce this bug

1. Open Firefox web browser.

2. Visit Utopian.io and log in.

3. Click '+ New Contribution' -- 'Development' -- 'I understand. Proceed'.

4. Click the 'Reward' button at the bottom of the new post web page


### Suggestions

The reward option menu should be close to the Reward button.

---

这是我提交给乌托邦的一个bug。我觉得帖子的标签光一个 utopian-io 就够了，可是发布时必须再填个标签。我想不出别的合适的标签，只好填了我爱的 cn 了，并且添上了这段中文文字，免得被小猎豹踩……

<br /><hr/><em>Posted on <a href="https://utopian.io/utopian-io/@dapeng/bug-hunting-the-reward-selection-menu">Utopian.io -  Rewarding Open Source Contributors</a></em><hr/>
