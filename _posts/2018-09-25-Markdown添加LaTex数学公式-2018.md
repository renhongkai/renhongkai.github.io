---
layout:     post
title:      Markdown添加Latex数学公式
date:       2018-09-25
author:     renhongkai
header-img: img/sourcetree/red_giant_hero.jpg
catalog: true
mathjax: true
tags:
    - software
---

> 这篇文章转载自[我在知乎上的回答](https://www.zhihu.com/question/51508063/answer/275401076)

严谨的证明的话，可以使用「形式语言」（[Formal language](https://en.wikipedia.org/wiki/Formal_language)）来证明：

在可计算理论和计算复杂度理论中，每个「计算问题」都被描述为一个一个「形式语言」，即字符串的集合。比如对于判断一个图是否是无向连通图这个问题：我们可以写为一个描述所有无向连通图的集合：

$$
A = \{ \langle G \rangle \vert G \text{ is a connected undirected graph}\}
$$

由于图灵机只能接受字符串，所以这里的尖括号表示对图的「编码」。出于简单，我们全部使用现实计算机所使用的字母表
$\Sigma = \\{0, 1\\}$，所以「编码」即一个对象的二进制字符串描述。

如果我们能构造出一个图灵机来「决定」这个「形式语言」，即可以判断一个「输入」是否属于这个集合（membership 与 non-membership），那么我们可以说我们用「图灵机」描述了一个「算法」来计算这个问题，而这个「计算问题」所对应的函数是「可计算的」，否则是「不可计算的」。（注 1）
