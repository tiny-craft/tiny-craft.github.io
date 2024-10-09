---
title: Tiny RDM：你的下一代Redis桌面GUI神器
categories: 文章
date: 2024-01-13 18:30:09
tags:
    - Tiny RDM
---
>开源/免费/高颜值/跨平台/轻量/功能齐全，集众多优点于一身的Redis GUI工具，你确定不试用一下吗？

## 简介

相信对Redis有频繁操作需求的用户，大部分会选择一个顺手的图形化界面工具来代替手动命令行操作以提高效率。Tiny RDM（Tiny Redis Desktop Manager）就是这么一款桌面端工具， **开源/免费/高颜值/跨平台/轻量/功能齐全**，不输当今市面同类主流产品。
![light_zh.png](light_zh.png)

## 功能特色

- **极致轻量且跨平台**：支持macOS、Windows和Linux操作系统，所有平台的安装包均在10M左右，随处安装随处运行。![download_list.png](download_list.png)
- **现代化界面**：符合现代审美的简洁界面，提供浅色/深色主题。![light_zh2.png](light_zh2.png)
- **丰富的登录方式和个性化连接设定**：支持SSH/SSL/哨兵/集群登录，同时提供系列个性化连接配置。![connection.gif](connection.gif)
- **支持多种格式查看**：内置高级文本代码编辑器，支持语法高亮/代码折叠/错误提示等功能，可轻松编辑及保存加密压缩内容。![format_change.gif](format_change.gif)
- **便捷搜索过滤**：使用正则匹配搜索键后，仍可进行二级过滤，组合筛选数据更方便。<img src="search_filter.gif" alt="search_filter.gif" width="300" />
- **支持海量键加载**：通过分段加载设定，无惧千万级别键值，外部键列表和复杂类型内部值（List/Hash/Set/ZSet/Stream）均默认开启。
- **数据批量操作**：可对键列表自定义多选，提供`数据导入导出`、`多选删除`、`正则匹配删除`、`批量更新TTL`等。
- **调试分析相关支持**：拥有`命令行`、`慢日志查询`、`服务器命令实时监控`、`发布/订阅`，极大提高Redis开发调试效率。![[debug_function.png]]
- **其他**：`数据库别名`、`自动刷新`、`可读性有效期`、`二进制键显示`、`多彩数据类型图标`、`TTL便捷设置标签`等等等等。开发者坚信，细节不一定会被肉眼注意到，但是一定能用心感受出来。

## 下载安装

> 1. Github下载地址：[github.com/tiny-craft/tiny-rdm/releases](https://github.com/tiny-craft/tiny-rdm/releases)
>
> 2. 官方微信公众号『独立开发记事簿』，输入关键字：`下载RDM`

`PS：目前官方没有和任何渠道合作（如果后续有的话会在项目README和公众号展示），请尽量通过官方仓库地址、官方微信公众号下载，或者源码自行编译安装。务必慎重从其他渠道下载安装，如因使用来路不明的安装包而造成损失，概不负责。`
## 结语

Tiny RDM是一款功能齐备的Redis客户端工具，完全可以满足日常开发和运维使用需要。该项目系开发者为爱发电的开源作品，有任何对项目有益的建议和反馈，欢迎到Github issue发表。
希望能为国产开源添砖加瓦，也可以给其他开发者提供价值。

> 官方地址：[redis.tinycraft.cc/zh/](https://redis.tinycraft.cc/zh/)
> 
> 源码地址：[github.com/tiny-craft/tiny-rdm](https://github.com/tiny-craft/tiny-rdm)
