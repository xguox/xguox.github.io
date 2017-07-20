---
layout: post
title: "Nginx 默认不允许 header 的 key 带下划线"
date: 2017-04-10 13:25:20
categories: Nginx
description:  underscores are forbidden in HTTP header names NGINX
---
<!--more-->


本地开发正常的很, 上到 staging 发现歇菜了, **request.env** 没找着自定义的 key, 折腾老久原来是 Nginx 给抹了.

= . =

##### 解决办法:

要不换个名, 要不加一句配置

```ruby
underscores_in_headers: on
```