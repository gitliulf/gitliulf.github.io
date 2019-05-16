---
title: unbuntu-apt 
date: 2019-05-16 13:02:07
tags: 
- linux
- ubuntu 
- apt 

categories:
- 技术文章

---
debian apt常见用法

# apt 命令
在Ubuntu下，apt-get近乎是最常用的shell命令之一了，因为他是Ubuntu通过deb安装软件的常用工具命令。

下面列举常用的 apt命令

- apt-cache search package 搜索软件包
- apt-cache show package  获取包的相关信息，如说明、大小、版本等
- **sudo apt-get install package 安装包**
- sudo apt-get install package --reinstall   重新安装包
- sudo apt-get -f install   修复安装
- **sudo apt-get remove package 删除包**
- sudo apt-get remove package --purge 删除包，包括配置文件等
- **sudo apt-get update  更新源**
- **sudo apt-get upgrade 更新已安装的包**
- sudo apt-get dist-upgrade 升级系统
- apt-cache depends package 了解使用该包依赖那些包
- apt-cache rdepends package 查看该包被哪些包依赖
- sudo apt-get build-dep package 安装相关的编译环境
- **apt-get source package  下载该包的源代码**
- sudo apt-get clean && sudo apt-get autoclean 清理无用的包
- sudo apt-get check 检查是否有损坏的依赖
