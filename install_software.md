---
title: Linux软件安装
date: '2017-05-22 23:12:29'
categories: []
layout: post
author: Yongxin Shi
description: Linux 安装软件一般有几种方式从软件源安装（软件商店），源码安装，二进制安装
slug: install_software
tags: []
draft: false
---

Linux软件安装
==========

## 软件
Linux 安装软件一般有几种方式从软件源安装（软件商店），源码安装，二进制安装

### 软件源安装
一般配置好源之后要更新源缓存
#### Ubuntu && debian

    sudo apt update

#### 关于apt-get aptitude
> deb 系的apt-get, aptitude, apt
>
> apt 是apt-get 封装
>
> 这两个工具使用，网上好多文章也没说清楚区别
>
> debian官方给出的解释是日常应用用aptitude
>
> aptitude 在日常使用会更有优势，他的包关系数据记录更优秀，不过这种优势只在一直用aptitude 才有
>
> 滚动升级时用apt-get，aptitude比较激进，不过对于桌面来说无所谓

#### apt-get 常用卸载参数
```sh

# 卸载软件包
apt remove 软件名

# 卸载软件包 和 只和这个软件包有依赖关系的包
apt autoremove 软件名

# 卸载软件包 和 只和这个软件包有依赖关系的包 和 配置文件
apt autoremove --purge 软件名
```

##### 参考文档
https://www.debian.org/doc/manuals/debian-reference/ch02.zh-cn.html#_literal_apt_get_literal_literal_apt_cache_literal_vs_literal_aptitude_literal

#### archlinux

    pacman -Sy

### 安装

    apt install 软件名

已Ubuntu为例：

    apt install sl

# 自己下载的软件包一般分成两类二进制包 源码包
一般都是.tar.gz tar.xz tar.bz2 tar 结尾的
先解压
    tar -xvf 你的软件包名.tar.gz

## 二进制包安装
一般先看README.md一般情况都是
    ./install

或者没有把安装文件打包的直接执行安装的可以把文件移动到/opt目录下
然后把建立软链接到$PATH路径理

    ln -s /opt/你的软件报名/启动程序名 /usr/bin

如果有.desktop结尾的文件可以

    cp /opt/你的软件包名/启动程序名.desktop /usr/share/applications/

## 源码包
一般都是有makefile文件的都是源码包

先安装编译基础工具如make gcc g++ 之类的软件
#### Ubuntu && debian
    apt-get install build-essential

#### archlinux
    pacman -S base-devel

### 编译三部曲
    ./configure
    make
    sudo make install
