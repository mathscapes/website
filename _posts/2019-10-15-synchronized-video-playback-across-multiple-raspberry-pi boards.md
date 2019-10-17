---
layout      : post
title       : Synchronized video playback across multiple Raspberry Pi boards
author      : "Gaurav Singh"
tags        : ["Python", "NewMedia", "RaspberryPi", "Video", "Synchronous"]
cite        : false
---

This project was done in collaboration with [Debanshu Bhaumik](https://bhaumikdebanshu.wixsite.com/portfolio), a Creative technologist & New media art practitioner. 

Popularity and power of single board computers like Raspberry Pi have made it possible not just to promote the teaching of basic computer science but also to prototype and in fact, to be even used by artists in their installations who often have particular requirements to be met. Boards like Raspberry Pi are quite capable and in many cases can substitute full PCs for such installations.

Playing single/multiple videos across multiple (and often large) displays require specialized hardware splitters and devices to read in video from a computer and then sent out to multiple devices in a synchronised manner. However, these devices are expensive and require an expert who has the know-how of using it. This small but meaningful realization by Debanshu eventually led us to build a simple API to facilitate synced video playback across multiple Raspberry Pi boards.

We have currently built a basic prototype of the implementation, and the following part of this post explains the working of it in detail. 

<img src="{{ site.baseurl }}/assets/images/svideo-architecture-01.svg" width="300px">
<figcaption>SVideo architecture</figcaption>

On one side, the boards are connected in a master-slave combination where the master computer controls the playback across the rest of the boards, which works in slave mode, each of the boards can be connected to any display device. The display devices may be placed in multiple configurations - from the standard grid to anything desired. The current implementation of the API does not do anything to the video file and uses pre-stored video files on the respective boards to playback in a synchronized manner. The current method can also extend to run a video file from the network or apply effects like cropping, video filters in near realtime.

The boards communicate over standard TCP/IP socket and get paired by a single handshake and tell the master computer whenever they are ready to start playback. Once all the slave computer responds with the available status, the master computer schedules or instructs all the slave computers to initiate the video playback. VLC player currently holds the video playback through the command line, which also removes any other screen to be displayed on the actual display, which otherwise is not relevant to the overall aesthetics/experience of the installation.

While the final fixes on the API are still coming through, we are happy to show you SVideo API, which is currently hosted [here](https://github.com/mathscapes/svideo). Feel free to check out and contact us for more information.