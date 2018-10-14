---
layout: post
title: "查看 TCP 端口号占用"
date: 2018-11-01 21:30:00
categories: Tools
tags: Tools
---

<!--more-->
查看 TCP 端口被哪个进程(PID)占用了

```go
lsof -nP -i4TCP:$PORT | grep LISTEN
```