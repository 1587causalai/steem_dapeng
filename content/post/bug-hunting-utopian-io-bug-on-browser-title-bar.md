---
title: "Bug Hunting: utopian.io bug on browser title bar"
author: dapeng
date: "2017-11-27 10:02:51"
slug: bug-hunting-utopian-io-bug-on-browser-title-bar
categories: [utopian-io]
tags: 
  - utopian-io
  - bug
---

原文链接: [steemit](https://steemit.com/utopian-io/@dapeng/bug-hunting-utopian-io-bug-on-browser-title-bar), [cnsteem](https://cnsteem.com/utopian-io/@dapeng/bug-hunting-utopian-io-bug-on-browser-title-bar), [busy](https://busy.org/utopian-io/@dapeng/bug-hunting-utopian-io-bug-on-browser-title-bar), [chainbb](https://chainbb.com/utopian-io/@dapeng/bug-hunting-utopian-io-bug-on-browser-title-bar), [steemdb](https://steemdb.com/utopian-io/@dapeng/bug-hunting-utopian-io-bug-on-browser-title-bar), [steemd](https://steemd.com/utopian-io/@dapeng/bug-hunting-utopian-io-bug-on-browser-title-bar), [busy](https://busy.org/utopian-io/@dapeng/bug-hunting-utopian-io-bug-on-browser-title-bar), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_dapeng/master/content/post/bug-hunting-utopian-io-bug-on-browser-title-bar.md)

## The bug: browser title bar of utopian.io not updated with the webpage

When I visit a user's homepage on utopian.io, the title bar always displays THIS user's name, no matter which page I have jumped to. In the following image, you can see that I jumped from @elear's home page to my own, but the title bar still displayed 'elear'.

[![utopianbug.jpg](https://res.cloudinary.com/hpiynhbhq/image/upload/v1511776892/gjiiane08jbuacycf3rh.jpg)](https://res.cloudinary.com/hpiynhbhq/image/upload/v1511776892/gjiiane08jbuacycf3rh.jpg)
*Click the image to zoom in.*

## My session information

Windows 7, Firefox 56.0 (32-bit)

## How to reproduce this bug

1. Open a web browser. Login utopian.io.

2. Type the web address https://utopian.io/@elear (don't click this hyperlink here) in the address bar and enter. You can see the title bar is 'elear'.

3. Click your own avatar on the topright. You see your homepage. The title bar displays your id. Wait seconds (the waiting time might depend on your computer). The title bar changes back to 'elear' automatically.

4. Click the utopian logo on the topleft. You see the home page of utopian. The title bar displays 'utopian'. Wait seconds. The title bar changes back to 'elear' automatically.

## Suggestions to fix

The title bar should display the title of the webpage which the user is browsing.

PS. @elear's homepage is used as an example in this post, just because elear gave me kind help on how to use utopian.io. Thanks a lot!

<br /><hr/><em>Posted on <a href="https://utopian.io/utopian-io/@dapeng/bug-hunting-utopian-io-bug-on-browser-title-bar">Utopian.io -  Rewarding Open Source Contributors</a></em><hr/>
