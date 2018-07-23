---
title: jekyll使用笔记
author: wanghao
date: 2018/07/13
tags: jekyll note
excerpt_separator: <!--more-->
---

jekyll基本用法
<!--more-->

# 启动本地服务
```ruby
#启动 ctrl+c关闭
bundle exec jekyll serve

#在后台启动
bundle exec jekyll serve --detach

#关闭后台服务器
pkill -f jekyll
#获取 PID
ps aux | grep jekyll
#kill 进程
kill -9 PID
```

### [jekyll中文文档](http://jekyllcn.com/docs/home/).


