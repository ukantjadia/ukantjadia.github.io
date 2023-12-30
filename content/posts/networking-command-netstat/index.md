---
title: Networking Command Netstat
seo_title: Networking Command Netstat | Linux
summary: Learn how to use `netstat` command
description: Learn how to use `netstat` command
slug: networking-command-netstat
author: Ukant Jadia

draft: false
date: 2023-12-30T14:14:11+05:30
lastmod: 
expiryDate: 
publishDate:  2022-05-25T22:33:19+05:30

feature_image: 
feature_image_alt: 

categories:
    - Basics
tags:
    - Networking
    - Linux
    - Basics
series:

toc: false
related: true
social_share: true
newsletter: false
disable_comments: false
---


# Learn Netstat 
> A basic `Linux` network command

## NETSTAT 

+ Prints the network connection and routing tables.
+ Like an CCTV monitor for every connection come in and go out from your machine.
+ MiniManual
>
> + `netstat -ant` : `a` for all connection, `n` for numeric, `t` for all TCP connection//`u` for the UDP connection
> + `netstat -rnec` :`r` for the route information, `n` numeric, `e` extend, `c` continous prints the result
> + `netstat -stuw` : `s` for statistics summary,`t/u` for tcp/udp, `w` prints raw data
> + `netstat -tulpn` : it shows the connectio with PID numbers
> + `lsof -i` : it establish the connection 
