---
title: app-reset-design
date: 2019-04-25 03:38:28
tags:
- restify

categories:
- 技术文章

---
定义apiResultFull api


# 根据resetfull API 规范定义一个自己的 api规范
定义格式如下
 > /app/userid/resname
 > GET    查询
 > POST   新增
 > PUT    修改
 > DELETE 删除

所有请求使用http中请求类型表示其目的
url只定义资源的路径
包含一下几个动作类型
资源服务器提供登录验证
资源服务器提供版本支持和不同格式的请求
第一个版本只提供json的格式请求

