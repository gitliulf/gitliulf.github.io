---
title: app-reset-design
date: 2019-04-25 03:38:28
tags:
- node
- restify

categories:
- 技术文章

---


根据resetfull API 规范定义一个自己的 api规范

定义格式如下
 > /app/userid/resname

所有请求使用http中动作表示其目的

url只定义资源的路径

包含一下几个动作类型

> GET、POST、PUT和DELETE

资源服务器提供登录验证

资源服务器提供版本支持和不同格式的请求

第一个版本只提供json的格式请求

