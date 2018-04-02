---
layout:     post
title:      "Hello Github Pages"
subtitle:   " \"Hello World, Hello Blog\""
date:       2018-03-28 12:00:00
author:     "BlackBeans"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 生活
---

> “So, That's it. ”


## 前言

BlackBeans 的 Blog 就这么开通了。

[跳过废话，直接看技术实现 ](#build) 



2018 年，BlackBeans 终于决定整一个自己的博客，在这里记录自己的学习心得 & 生活点滴。

2018年03月27号，在整理笔记的时候发现有点乱，不方便维护和回顾，所以萌生了整理博客的想法，便于在学习东西的时候多反思、多总结，之前有写CSDN等通用平台的博客，毕竟是第三方的东西，不是自己折腾起来的，维护的意愿不强烈。感觉Github Pages + Jekyll的方式整个自己的博客成本也不大，干脆整一个玩玩。

首先需要声明的是：本博客借鉴了github上的开源博客框架，在这里要感谢[huangxuan](http://huangxuan.me/)， [github地址](https://github.com/Huxpro/huxpro.github.io)。



<p id = "build"></p>
---

## 正文


接下来说说搭建这个博客的技术细节。  

正好之前就有关注过 [GitHub Pages](https://pages.github.com/) + [Jekyll](http://jekyllrb.com/) 快速 Building Blog 的技术方案，非常轻松时尚。

其优点非常明显：

* **Markdown** 带来的优雅写作体验
* 非常熟悉的 Git workflow ，**Git Commit 即 Blog Post**
* 利用 GitHub Pages 的域名和免费无限空间，不用自己折腾主机
	* 如果需要自定义域名，也只需要简单改改 DNS 加个 CNAME 就好了 
* Jekyll 的自定制非常容易，基本就是个模版引擎


---

配置的过程中也没遇到什么坑，基本就是 Git 的流程，相当顺手

大的 Jekyll 主题上直接 fork 了 Clean Blog

中文字体的渲染，fork 了 [Type is Beautiful](http://www.typeisbeautiful.com/) 的 `font` CSS

本地调试环境mac:
 `brew install ruby`
 `sudo gem install jekyll`
 `sudo gem install jekyll-paginate`
 `jekyll serve`

## 后记

该博客框架的作者现在已经是业内大牛，本人的目的是整个自己写东西的空间，所以并未在框架搭建上耗费太多精力，开源是技术进步的助力，再次向huangxuan先生致谢。






