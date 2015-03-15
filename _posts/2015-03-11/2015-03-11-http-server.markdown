---
layout: post
title: python http server
category: itbasic
tags: [http]
---
python可以非常方便的启动一个微型的HTTP服务程序。可以用于把当前目录网络共享出去。
python -m SimpleHTTPServer 后接端口号
可以加入alias，方便使用。
alias http = 'python -m SimpleHTTPServer'
以后可以直接http 2000,就可启动一个端口2000的http server.
