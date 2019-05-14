---
title: npm 使用国内源 
date: 2019-04-30 01:23:37
tags: 
- node

categories:
- 技术文章

---

切换npm使用的源地址

## Node 的官方模块仓库网速太慢，模块仓库需要切换到阿里的源。
不安装 cnpm 只用淘宝镜像，设置 npm 的镜像：
$ npm config set registry https://registry.npm.taobao.org/
执行下面的命令，确认是否切换成功。
$ npm config get registry
