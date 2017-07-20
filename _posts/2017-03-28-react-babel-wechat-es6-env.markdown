---
layout: post
title: "weixin://preInjectJSBridge/fail [React]"
date: 2017-03-28 23:25:20
categories: [JavaScript, React]
tags: [JavaScript, React]
---
<!--more-->


**Redux** 中 reducer 返回 state 的时候经常用到 Object.assign， 然后几乎所有现代浏览器都试过能正常运行以后， 发现在微信的内置浏览器里边就报这玩意，

**weixin://preInjectJSBridge/fail**

babel 没把该语法翻译成微信认识的，添加 **babel-polyfill** 这个库， webpack 入口配置一下， 就可以解决了。

