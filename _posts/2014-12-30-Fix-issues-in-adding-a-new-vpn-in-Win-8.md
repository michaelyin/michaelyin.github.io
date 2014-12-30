---
layout: post
title: Fix issues in adding a new VPN client in Windows 8
---

I am testing a Java program which needs to operate on a website deployed in China. I don't have control on that website. And
at some point of the operations, the website rejects me because it only allows traffic inside China.

I quickly set up a OpenVPN server on a box in China. But when I tried to add a new vpn connection on my Win 8 box, the connection 
can be added smoothly. But it does not show up in the networking list.

How to fix it?

1. open Windows PowerShell
2. type Remove-VpnConnection in your shell
3. type your vpn connection name for deletion
4. re-create your vpn connection

The issue is probably caused by a bug in the wi-fi interface on the Win 8 box. If you encounter the similar issue, you can 
give it a try.
