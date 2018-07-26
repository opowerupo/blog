---
title: Gradle 笔记
author: wanghao
date: 2018/07/26
tags: Study Gradle
excerpt: 学习和使用过程中的一些记录
---

当使用了SpringBoot的起步依赖时，Gradle倾向于使用库的最新版本，所以要将起步依赖中的某个依赖替换成老版本时，
需要先排除掉起步依赖中的那个版本 例：
```groovy
compile('org.springframework.boot:spring-boot-starter-web'){
    exclude group:'com.fasterxml.jackson.core'
}
compile('com.fasterxml.jackson.core:jackson-databind:2.3.1')
```