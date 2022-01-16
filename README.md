﻿# XNetcat
## 简介
- 基于Python的Netcat, 用于外带数据攻击.

## 作用
- 类似于 ncat -l -k -v -o netcat.log --append-output -p 4444
- 监听端口, 获取接收到的数据.
- 保持端口监听, 可收到客户端多次新建的请求.
- 收到请求后立即断开, 避免占用靶机的程序线程和网络连接.
- 记录历史请求, 保存请求原文.

## 优点
- 代码开源, 安全可控.
- 不依赖第三方库.
- 跨平台.
- 解决了内网环境无法下载ncat的问题.
- 解决了ncat命令过于冗余的问题.
- 解决了ncat监听模式下需要频繁ctrl+c才能终止oob连接的问题.
