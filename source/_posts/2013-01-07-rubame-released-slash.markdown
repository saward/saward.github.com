---
layout: post
title: "Rubame released!"
date: 2013-01-07 15:16
comments: true
categories: [Ruby, Programming]
---

The first release of [Rubame](https://saward.github.com/Rubame) is out.  I wanted a simple websocket alternative to EventMachine that would give me more control over my game server's main loop, such as controlling precisely when the network server loop is called.  Ideally now I will be able to use fibers more effectively to allocate cpu resources where they are most needed at the time.  That is, when the server has a lot of work to do, it can still ensure that the network code is called regularly without tying up the system too much.  That's the hope, anyway!