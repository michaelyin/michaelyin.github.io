---
layout: post
title: Fix Himedia tvmc video playing crash
---

When the tvmc is loading a video, the whole application crashes without any trace. 

It is caused by the Hardware acceleration settings. Just uncheck the mediacodec, the issue would be gone.
System -> Settings -> Video

系统-设置-视频:
设置级别-->专家
加速-->UNCHECK mediacodec
