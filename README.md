# shell介绍

## 1.shell

Shell 是指一种应用程序，由 C 语言编写，这个应用程序提供了一个界面，用户通过这个界面访问操作系统内核(Kernel)的服务。



![shell](assets/shell.png)



## 2.Shell 脚本

Shell 脚本（shell script），是一种为 shell 编写的脚本程序。

业界所说的 shell 通常都是指 shell 脚本，但读者朋友要知道，shell 和 shell script 是两个不同的概念。

由于习惯的原因，简洁起见，本文出现的 "shell编程" 都是指 shell 脚本编程，不是指开发 shell 自身。



## 3.Shell 的种类

- Bourne Shell（/usr/bin/sh或/bin/sh）
- Bourne Again Shell（/bin/bash）
- C Shell（/usr/bin/csh）等等

可以通过 

**cat /etc/shells** 命令来查看系统的shell种类

**echo $SHELL** 命令来查看当前使用的shell

![image-20230817110032065](assets/image-20230817110032065.png)



## 4.shell 的历史

![img](assets/webp.webp)

### Unix与shell

1970年，Kenneth Thompson(贝尔实验室)和Dennis Ritchie(贝尔实验室) 使用汇编语言开发的UNIX系统投入运行。

1971年，Ken Thompson为UNIX开发了第一种shell，称为V6 shell。这个版本shell的缺陷在于脚本编程能力的不足，它只是一个交互性的命令解释器。

1972年，DennisRitchie开发出C语言，用来重写了UNIX，由此产生了UNIX VersionV。

1977年，Stephen Bourne在贝尔实验室使用C语言为V7 UNIX开发了Bourne Shell，bshell一直沿用至今。



### Linux与bash 

1989年，Brian Fox(贝尔实验室)开发了Bourne-Again Shell，即bash，是GNU的项目，旨在替换Bourne Shell。之后bash成为了在Linux上最流行的shell，并成为许多Linux发行版默认的交互式shell。



### 扩展阅读

#### ash

1989 年，Almquist(贝尔实验室)开发的ash发布，是unix的shell，具有 System V shell 的大部分功能。ash 速度快、体积小，它非常适合内存较低的机器，但是功能没有shell全。后来ash又有了很多衍生版本，被安装在FreeBSD、NetBSD等Linux的发行版上，作为默认 shell (/bin/sh) 。

#### dash

1997 年，Herbert Xu 将 Ash 从 NetBSD 移植到 Debian Linux。

2002 年 9 月发布 0.4.1，该端口被重命名为 Dash（Debian Almquist shell）

2006 年，Ubuntu 决定采用 Dash 作为默认的 /bin/sh，使用 Dash 的原因是 shell 脚本运行得更快，特别是在操作系统启动时。但是，交互式使用的默认登录 shell 仍然是 Bash。

![image-20230817112032988](assets/image-20230817112032988.png)

Ash（主要是 Dash 分支）在嵌入式 Linux 系统上也很流行。 Dash 版本 0.3.8-5 内置于 BusyBox中，并可与 DSLinux、Alpine Linux、Tiny Core Linux 以及基于 Linux 的版本（例如 OpenWrt、Tomato 和 DD）配合使用。

#### ksh

1983年，Korn(贝尔实验室)发布了Korn shell，基于Bourne shell的源代码发展而来，KornShell是向后兼容的Bourne Shell。

#### mksh

 Android 在 Android 4.0 之前使用 Ash，但在 Android 4.0 之后改用 mksh。















