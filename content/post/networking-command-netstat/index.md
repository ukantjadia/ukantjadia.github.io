---
title: Networking Command Netstat
subtitle: Learn how to use `netstat` command

summary: Learn how to use `netstat` command

draft: false
date: 2023-12-30T14:14:11+05:30
lastmod: 


categories:
    - Basics
tags:
    - Networking
    - Linux
    - Basics
projects: []
featured: false
# authors:
#   - Ukant Jadia


image:
  caption: ''
  focal_point: ''
  placement: 2
  preview_only: false
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
