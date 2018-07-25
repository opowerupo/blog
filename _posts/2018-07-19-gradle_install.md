---
title: Gradle 安装
author: wanghao
date: 2018/07/19
tags: Study Gradle
excerpt: Gradle安装工具和流程
---

### 1.使用包管理工具安装
>[SDKMAN](https://sdkman.io/)
(The Software Development Kit Manager)
是一个用来在类unix操作系统(如mac,Linux等)中进行多版本切换、安装和卸载工作的工具
```shell
❯ sdk install gradle
```
>[Homebrew](https://brew.sh/)
是Mac OSX上的软件包管理工具,能在Mac中方便的安装软件或者卸载软件，相当于linux下的apt-get、yum神器
```shell
❯ brew install gradle
```
>[Scoop](https://scoop.sh/)
是windows上个一个包管理工具，通过scoop能快速在机器上安装所需要的标准工具、自定义工具
```shell
❯ scoop install gradle
```
>[Chocolatey](https://chocolatey.org/)
是windows上个一个包管理工具
```shell
❯ choco install gradle
```

### 2.手动安装
>**第一步 [下载](https://gradle.org/releases/?_ga=2.188391976.1841367415.1532311454-1388520471.1531906837) 
最新版本的安装包**

>**第二步 解压Gradle**
>> **_Linux & MacOs 用户_**
```shell
❯ mkdir /opt/gradle
❯ unzip -d /opt/gradle gradle-4.9-bin.zip
❯ ls /opt/gradle/gradle-4.9
```
>> **_Windows 用户_** 
<br>
创建一个文件夹C:\Gradle 后面解压ZIP包等工作请自行脑补^^

>**第三步 配置环境变量**
>> **_Linux & MacOs 用户_**
```shell
❯ export PATH=$PATH:/opt/gradle/gradle-4.9/bin
```
>> **_Windows 用户_** 
<br>
添加一个 GRADLE_HOME 环境变量来指明 Gradle 的安装路径 
<br>
添加 GRADLE_HOME/bin 到 PATH 环境变量中.

### 3.测试安装结果
```
❯ gradle -v
                                                                       ` 
-------------------------------------------------------------------
Gradle 4.9
------------------------------------------------------------------- 
                                                                       ` 
Build time:   2018-07-19 08:14:03 UTC
Revision:     819e0059da49f469d3e9b2896dc4e72537c4847d
                                                                       `         
Kotlin DSL:   0.18.4
Kotlin:       1.2.41
Groovy:       2.4.1
Ant:          Apache Ant(TM) version 1.9.11 compiled on March 23 2018
JVM:          1.8.0_66 (Oracle Corporation 25.66-b17)
OS:           Mac OS X 10.11.6 x86_64
```

* 以上是Gradle的安装，摘自[Gradle官网](https://docs.gradle.org/current/userguide/installation.html).



