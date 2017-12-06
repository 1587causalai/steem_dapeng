---
title: "mindr: an R package that creates a markdown post out of a mind map - 将帖子转成思维导图"
author: dapeng
date: "2017-12-02 17:20:15"
slug: mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map
categories: [utopian-io]
tags: 
  - utopian-io
  - cn
  - programming
  - cn-reader
  - steemit
---

原文链接: [steemit](https://steemit.com/utopian-io/@dapeng/mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map), [cnsteem](https://cnsteem.com/utopian-io/@dapeng/mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map), [busy](https://busy.org/utopian-io/@dapeng/mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map), [chainbb](https://chainbb.com/utopian-io/@dapeng/mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map), [steemdb](https://steemdb.com/utopian-io/@dapeng/mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map), [steemd](https://steemd.com/utopian-io/@dapeng/mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map), [busy](https://busy.org/utopian-io/@dapeng/mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_dapeng/master/content/post/mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map.md)

This post was written bilingually, in English and Chinese.

> 本文用英文和中文写作，中文在后半部分。

## Introduction

### Background 

A mind map is a diagram used to visually organize information. Markdown is a markup language widely used for writing, for example, posts on steem and Utopian.io.

This post is to introduce an open-source package called ***[mindr](https://github.com/pzhaonet/mindr)*** I have been developing with R language for creating mindmaps from markdown posts, or vice versa. 

### Motivation

If you are a mindmap fan, you might start an Utopian.io post from a mindmap like this:

![Submit to Utopian.jpg](https://res.cloudinary.com/hpiynhbhq/image/upload/v1512234540/rsa2ssccr6xw4nbyvjas.jpg)

Yes, this is the structure of this post. Maybe it could be a template for Utopian.io.

The mindmap helps organize your idea. Now you start writing your post. Isn't boring if you have to type the same words in the mindmap again?

On the other way around, if you have already written a post, wouldn't it be amazing if you present the outline of the post  in a nice mindmap?

## Features

With R mindr package, these tasks can be done with one single command.

### Markdown to Mindmap

mindr can convert a markdown file or multiple markdown files, such as steem posts, into one mindmap, which could be opened and edited with common mindmap software like Freemind and Xmind.

### Mindmap to Markdown

mindr can also convert a mindmap into a markdown file, which can be a good start of your post.

### Outline

If you don't like mindmaps, you can use mindr just to extract the outline from your markdown file(s).

## Quick Start

### Installation of R

[Download R](https://cran.r-project.org) and install it.

### Installation of mindr

In R environment, run the following codes to install mindr.

```
# stable version:
install.packages("mindr")
# or development version:
devtools::install_github("pzhaonet/mindr")
```

### Examples

As an example from markdown to mindmap, run:

```
library('mindr')
example(md2mm)
```

then you will get a demo mind map file mindr.mm in the working directory (getwd()). Open it with any mind-map (brainstorm) software, and you will get a mind map.

As an example from mindmap, run:

```
example(mm2md)
```

then you will get a demo markdown file mindr.md in the working directory (getwd()).

Days ago I introduced the R package bookdownplus. From a book by bookdownplus or bookdown, you can simply get a mindmap with mindr. For example, if you throw the markdown files of the repo rstudio/bookdown into a folder and run mindr, you will get a mindmap like this:

![](https://raw.githubusercontent.com/pzhaonet/mindr/master/showcase/mindr_bookdown.jpeg)

## Link to the Repo

https://github.com/pzhaonet/mindr

## Proof of Work

The following images are screenshots  showing I am the author 'pzhaonet' of mindr.

![mindr.jpg](https://res.cloudinary.com/hpiynhbhq/image/upload/v1512303284/kapq7allgsxifomwaylf.jpg)

![image.png](https://res.cloudinary.com/hpiynhbhq/image/upload/v1512394305/uncwrp9nyslzj8ta0h0c.png)

## Conclusion

All I wanted to say is: mindr is a useful package for steemians who take writing serious.

---

本文介绍的是我开发的一个开源免费的 R 扩展包，唤作 mindr，用来在思维导图和 markdown 之间转换。


如果你是个思维导图粉丝，写帖子之前，可以用思维导图来组织一下思路，像上面第一幅图那样。


思路清晰了，现在开始按思路写文章。但是，你难道还想把图里的文字再重复敲一遍吗？


反过来也是。当你已经写好了帖子，如果能一下就把帖子转成一??思维导图，向别人展示帖子的结构和思路，岂不是一件美事？

mindr，助你轻松实现这些梦想。

只需先安装 R 语言环境，再按上文介绍的代码安装 mindr 扩展包，就可以得到上文展示的示例。

来试一下 mindr 吧！


<br /><hr/><em>Posted on <a href="https://utopian.io/utopian-io/@dapeng/mindr-an-r-package-that-creates-a-markdown-post-out-of-a-mind-map">Utopian.io -  Rewarding Open Source Contributors</a></em><hr/>
