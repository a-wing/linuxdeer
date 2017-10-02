---
title: Linux分区方案
date: '2017-06-06 23:12:29'
categories: []
layout: post
author: Yongxin Shi
description: 关于linux分区，各分区应该如何划分
slug: parted
tags: []
draft: true
---

Linux分区方案
==========

关于linux的分区，有好多初学者会纠结这个问题，网上给出的方法很多，有很多不一样的，主要是随着时间的流逝，有些教程太老了也不符合这个时代，大多数都是关于服务器方面的分区方法

## swap
swap 该多大？这是个问题。关于swap是什么。请自行百度

硬盘大的同学可以不考虑，直接把swap划到内存的2倍

其实以目前pc来看swap存在的意义不大，因为内存已经足够大了，swap可能都用不上了
以前看过大神写的文章说swap利用率最高是2倍内存的60%。就是 mem×2×60% = swap
反正我目前就是这么分的

8G以上的个人pc，如果没有特别需求，根本不需要swap

## home
如果作为桌面使用强烈建议把/home单独分出来

## boot
如果不用什么特殊的文件系统没必要单独分出来
