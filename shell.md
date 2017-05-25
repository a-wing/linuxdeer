Linux shell
==========


Shell是系统的用户界面，提供了用户与内核进行交互操作的一种接口。它接收用户输入的命令并把它送入内核去执行。
实际上Shell是一个命令解释器，它解释由用户输入的命令并且把它们送到内核。不仅如此，Shell有自己的编程语言用于对命令的编辑，它允许用户编写由shell命令组成的程序。Shell编程语言具有普通编程语言的很多特点，比如它也有循环结构和分支控制结构等，用这种编程语言编写的Shell程序与其他应用程序具有同样的效果。

### 常见shell
* bash
* csh
* ksh
* tcsh
* fish
* zsh
* elvish


#### bash --默认的shell
bash 是一个为GNU计划编写的Unix shell。它的名字是一系列缩写：Bourne-Again SHell — 这是关于Bourne shell（sh）的一个双关语（Bourne again / born again）。Bourne shell是一个早期的重要shell，由史蒂夫·伯恩在1978年前后编写，并同Version 7 Unix一起发布。bash则在1987年由布莱恩·福克斯创造。在1990年，Chet Ramey成为了主要的维护者。
bash是大多数Linux系统以及Mac OS X默认的shell。

bash 有自动补全工具bash-completion

    apt-get install bash-completion


#### zsh --最终的shell
默认的一般都是bash。一般要先安装zsh
设置默认shell

    apt-get install zsh
    chsh
##### 插件oh-my-zsh
https://github.com/robbyrussell/oh-my-zsh
