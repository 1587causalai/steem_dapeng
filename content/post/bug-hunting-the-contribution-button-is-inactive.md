---
title: "Bug Hunting: the '+Contribution' button is inactive on Ubuntu"
author: dapeng
date: "2017-12-22 10:48:57"
slug: bug-hunting-the-contribution-button-is-inactive
categories: [utopian-io]
tags: 
  - utopian-io
  - test
---

原文链接: [steemit](https://steemit.com/utopian-io/@dapeng/bug-hunting-the-contribution-button-is-inactive), [cnsteem](https://cnsteem.com/utopian-io/@dapeng/bug-hunting-the-contribution-button-is-inactive), [busy](https://busy.org/utopian-io/@dapeng/bug-hunting-the-contribution-button-is-inactive), [chainbb](https://chainbb.com/utopian-io/@dapeng/bug-hunting-the-contribution-button-is-inactive), [steemdb](https://steemdb.com/utopian-io/@dapeng/bug-hunting-the-contribution-button-is-inactive), [steemd](https://steemd.com/utopian-io/@dapeng/bug-hunting-the-contribution-button-is-inactive), [busy](https://busy.org/utopian-io/@dapeng/bug-hunting-the-contribution-button-is-inactive), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_dapeng/master/content/post/bug-hunting-the-contribution-button-is-inactive.md)

Update: after I posted this report, I saw that [the similar bug](https://utopian.io/utopian-io/@ah-2002/bug-hunting-contribution-add-contribution-button-on-the-top-is-not-working) was already reported three days ago. I am sorry that I missed it. However, the bug reported in my post was tested on different OS and different versions of the web browsers. Thus I think my report still makes sense.

### The bug: the '+Contribution' button on top of the webpage is inactive

There are two buttons on the home page of utopian.io for adding a new contribution. One is '+ New Contribution' on the left panel, and the other is a blue one called '+Contribution' on the top. See the screenshot.

![20171222-113811.jpg](https://res.cloudinary.com/hpiynhbhq/image/upload/v1513939718/nohm3tp8rtjiq5ac6nks.jpg)


I guess I should be able to add a new contribution by clicking either of them. However, the blue button is inactive. When I put my mouse on the blue button, the mouse shows a small hand, indicating that I could click. So I click it, but nothing happens.

It seems that the blue button is inactive.

### My session information

I tested it on both windows 7 + Firefox 56.0 (32-bit), and Ubuntu 16.04 + Firefox 57.0.1 (64-bit).

### How to reproduce this bug

1. Open Firefox web browser.

2. Visit Utopian.io and log in.

3. Click the blue button '+ Contribution' on the top-right.


### Suggestions

The blue button '+Contribution' should be active.

<br /><hr/><em>Posted on <a href="https://utopian.io/utopian-io/@dapeng/bug-hunting-the-contribution-button-is-inactive">Utopian.io -  Rewarding Open Source Contributors</a></em><hr/>
