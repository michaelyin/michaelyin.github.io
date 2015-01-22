---
layout: post
title: resize a sdhc micro card with Vmware Ubuntu
---

I need resizes the micro card being used on my raspberry pi.

I only have a Win 8 machine with Ubuntu virtual instance. so we can use the virtual instance to perform the task. 

First, follow this blog to access the micro card from your Ubuntu:
http://tomearp.blogspot.com/2014/01/using-sd-card-with-vmware-workstation.html

To find out your harddisk name: 
Start "RUN" in Windows-8 with keys [Win-Logo]+[R] and type in »(Edit-Box) "compmgmt.msc" and 
press [ENTER] to RUN the "Computer Management" in Windows-8.

When the micro card is available in Ubuntu, first install GParted. And now you can use GParted 
to handle your sd card.
