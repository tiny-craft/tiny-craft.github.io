---
title: Tiny RDM春节后第一个版本发布，支持自定义解码了
categories: 文章
tags:
  - Tiny RDM
  - 开源
abbrlink: '56988082'
date: 2024-02-22 11:36:22
---
春节后的第一个版本，除了修复了节前屯的众多bug以外，也带了不少新特性，又是一个具有历史意义的版本，加了众多新功能，新一年我真的不能再只埋头写代码了😂。

### 自定义编码解码

现在支持添加自定义编码，从此你使用任何离奇古怪加密方式的内容，都可以通过自定义解码来展示和编辑保存了。同时也能为更多和特定开发语言相关的序列化/反序列化提供原生级的解码，不用再担心用Golang强行解码的内容和预期不符了~
![自定义编码列表.png](自定义编码列表.png)
![新增和编辑解码编码器.png](新增和编辑解码编码器.png)
自定编码怎么使用？使用文档还没空写，着急用的小伙伴可以先看下源码实现，其中PHP和Pickle解码都是基于自定义解码实现的😂~

### 内嵌更多常用解码器（Msgpack/PHP/Pickle）

因为有了基于命令行调用的自定义解码器，所以这里顺手提供了原生级PHP和Pickle的反序列化/序列化支持。***这里要注意的是，需要系统命令行可以执行`php`命令解码选择列表中才会有`PHP`选项，同理`Pickle`也需要`python`或者`python3`命令支持。***
![php.gif](php.gif)
### 支持使用Unix Socket连接服务端

支持通过UNIX方式连接服务端，当然了通过URL格式字符串来创建新连接也是支持的~
`unix://<user>:<password>@</path/to/redis.sock>?dial_timeout=3&read_timeout=6s&max_retries=2`
![socket连接.png](socket连接.png)

### 支持为每个连接配置HTTP/SOCKS5代理

现在可以为每个连接自行配置网络代理了，支持HTTP/HTTPS/SOCKS5/SOCKS5H~

![proxy.png](proxy.png)
### 支持查看和编辑RedisJSON类型数据

既然支持String类型的JSON，当然也要专门支持RedisJSON，使用前请确保你Redis服务器启用了reJSON模块，它的使用和String类型的JSON文本一样简单~

### 其他
紧急修复了大量“已知”的BUG，不少问题还是几个版本前可能就已经存在了，居然才被我发现，或者说才有用户来反馈。看来大部分用户还是没有深度使用，或者对软件的在意程度不高啊~反思反思。

### **下载安装**

> Github下载地址：[github.com/tiny-craft/tiny-rdm/releases](https://link.zhihu.com/?target=https%3A//github.com/tiny-craft/tiny-rdm/releases)  
> Gitee下载地址：[gitee.com/tiny-craft-zh/tiny-rdm/releases](https://gitee.com/tiny-craft-zh/tiny-rdm/releases)
> 
> 官方微信公众号『独立开发记事簿』，输入关键字：`下载RDM`  


### 写在最后
这个版本之后就开始尽量不加大的新功能了，接下来会以完善用户使用手册和修补陈年老BUG提高稳定性为主，也开始尝试一些对外宣传软件和获取更多目标用户，写文章/做展示视频等等。

同时欢迎大家加群加好友交流，微信公众号『独立开发记事簿』可以找到我~

> 官方地址：[redis.tinycraft.cc/zh/](https://redis.tinycraft.cc/zh/)
> 
> 源码地址：[github.com/tiny-craft/tiny-rdm](https://github.com/tiny-craft/tiny-rdm)
