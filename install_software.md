Linux软件安装
==========

## 软件
Linux 安装软件一般有几种方式从软件源安装（软件商店），源码安装，二进制安装

### 软件源安装
一般配置好源之后要更新源缓存
#### Ubuntu && debian

    sudo apt update

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

    cp /opt/你的软件报名/启动程序名.desktop /usr/share/applications/

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
