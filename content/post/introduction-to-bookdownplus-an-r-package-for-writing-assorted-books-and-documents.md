---
title: "Introduction to bookdownplus: an R package for writing assorted books and documents"
author: dapeng
date: "2017-11-26 21:21:21"
slug: introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents
categories: [utopian-io]
tags: 
  - utopian-io
  - cn
  - programming
  - cn-reader
  - blog
---

原文链接: [steemit](https://steemit.com/utopian-io/@dapeng/introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents), [cnsteem](https://cnsteem.com/utopian-io/@dapeng/introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents), [busy](https://busy.org/utopian-io/@dapeng/introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents), [chainbb](https://chainbb.com/utopian-io/@dapeng/introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents), [steemdb](https://steemdb.com/utopian-io/@dapeng/introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents), [steemd](https://steemd.com/utopian-io/@dapeng/introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents), [busy](https://busy.org/utopian-io/@dapeng/introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_dapeng/master/content/post/introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents.md)

Hi guys! This is my first post on utopian.io. Hopefully it goes on the right way. This post was written bilingually, in English and Chinese.

> 嘿，你好！这是我在 utopian.io 发布的第一篇帖子。但愿我的发布方式没出什么叉子。本文用英文和中文写作，中文在后半部分。

This post is to introduce an open-source package called ***[bookdownplus](https://github.com/pzhaonet/bookdownplus)*** I have been developing with R language for writing assorted books and documents in bookdown environment. 

If you are a Steemian, or a markdown user, you might want to organize your posts in a friendly and elegant way. As far as I know, R *[bookdown](https://bookdown.org/yihui/bookdown/)* package is the best tool to convert markdown files into a nice book. However, *bookdown* is not easy for beginners. An R beginner might be confused or depressed in struggling in the flood of LaTeX, YAML, Markdown, Pandoc, etc. 

*bookdownplus* is the easiest shortcut to the world of *bookdown*. With **just one single command** users can get a demo book (or multiple demo books) in pdf, Word document, html, epub, or even more formats. *bookdownplus* extends the features of *bookdown*, and simplifies the procedure. Users only have to choose a template, clarify the book title and author name, and then focus on writing the text. No need to struggle in YAML and LaTeX. 

Multiple templates are included in *bookdownplus*. With these templates *bookdownplus* helps you write academic journal articles, guitar books, chemical equations, mails, calendars, diaries, etc.. For instance, the theisis_classic can convet your markdown file into a pdf book like this:

![](https://raw.githubusercontent.com/pzhaonet/bookdownplus/master/inst2/showcase/bookdownplus_thesis_classic.jpg)

and the poem template can make a nice poem book like this:

![](https://raw.githubusercontent.com/pzhaonet/bookdownplus/master/inst2/showcase/bookdownplus_poem.jpg)

Even a book with guitar chords:

![](https://raw.githubusercontent.com/pzhaonet/bookdownplus/master/inst2/showcase/bookdownplus_guitar.jpg)

If you have programing codes especially R codes in your posts, they can be integrated into your book in a reproducible way owing to the feature of R markdown, which looks like this:

![](https://raw.githubusercontent.com/pzhaonet/bookdownplus/master/inst2/showcase/bookdownplus_nonpar.jpg)


Wouldn't it be cool to make your steem posts into such a book?

Enjoy R *bookdownplus* !

本文介绍的是我开发的一个开源程序包，唤作 ***bookdownplus***，可以在 R 语言环境下制作各种书籍和文档。

如果你是 steem 或者 markdown 用户，你可能会想把你的帖子整理成一本漂亮的书跟别人分享。据我所知。R *['bookdown'](https://bookdown.org/yihui/bookdown/)* 是将 markdown 格式的文件转化成书的最佳工具。可惜的是，*bookdown* 并不容易上手。R 语言初学者可能要为 LaTeX, YAML, Markdown, Pandoc 等折腾很久，也享受不到 bookdown 带来 的快乐。

于是我开发了 bookdownplus。

bookdownplus 是对 bookdown 的增强和简化, 是快速使用 bookdown 的最简洁方法。bookdownplus 提供了很多有用的模板，可以很方便地在 bookdown 平台写文集、期刊论文、学位论文、学术海报、化学分子式、信件、日记、日历、诗集、吉他谱等各种常用文档和书籍。这是功能上的增强（+）。bookdownplus 使用时只需指定一个模板，给定作者和书名，就可以一键生成模板文件，用户在模板文件里照猫画虎写自己的文字就可以了，不必再花力气上网找模板、设置 YAML 和 LaTeX。这是操作上的简化（-）。

上???给了几个图示，分别展示了 bookdownplus 生成的文章合集、诗集、吉他谱、编程书籍的示例。

怎么样，快来用 bookdownplus 把你的 steem 帖子做成一本漂亮的书吧!

<br /><hr/><em>Posted on <a href="https://utopian.io/utopian-io/@dapeng/introduction-to-bookdownplus-an-r-package-for-writing-assorted-books-and-documents">Utopian.io -  Rewarding Open Source Contributors</a></em><hr/>
