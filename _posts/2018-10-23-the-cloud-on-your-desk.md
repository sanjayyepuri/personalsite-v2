---
layout: post
title: "The Cloud on Your Desk"
description: "Building a Cluster of Raspberry Pis"
image: "/assets/pi-cluster-build.jpeg"

category: 
tags: []
---
> Building a Cluster of Raspberry Pis

# Introduction
A year ago at a hackathon an engineer had demoed what he called the "cloud on your desk." Essentially it was  5 Raspberry Pis that were physically attached together on a frame with a network switch. Running on them was a software called OpenStack, a system designed to control compute, storage, and networking resources in large data centers that would be used by cloud applications. I found the compact device extremely interesting and felt that this was something I could do myself. But it wasn’t until earlier this year that I took up the challenge to build my own cluster. 

During spring break I decided to build a Pi cluster and have my own distributed computing test platform. I wanted to be able test various algorithms related to distributed systems (and maybe while it’s idle run a server or use it as a network share for our apartment). This was pretty different from the ideal of having the “cloud on your desk,” but it’ll be an interesting project. 

# The Build 
After I had looked online at other Pi clusters (such as this [one](https://makezine.com/projects/build-a-compact-4-node-raspberry-pi-cluster/) on Makezine), I decided I needed around 4-5 Raspberry Pis, a USB charging hub, and a network switch. Most any USB hubs and network switches should do; here are the specific ones that I bought. 

* 5x Raspberry Pi 3 B+
* 1x Anker 7 port USB Charging Hub 
* 1x Netgear FS108 8-port Network Switch
* 5x 6in. Ethernet Cables 
* 5x 6in. MicroUSB Cables 
* 5x 16GB microSD cards 

I then 3D printed [this](https://www.thingiverse.com/thing:1573414) stackable chassis for the Pis which I attached to the switch using a special permanent 3M tape. The end result was a little messy because I had run out of plastic towards the end of the print however the cluster was still functional. In fact this had allowed me to later borrow a friends Pi screen to attach to the top of the cluster (the cherry on top). This is how it turned out:

![](/assets/pi-cluster-build.jpeg)

# Next Steps 
Since the spring after I had assembled the components, I've been swamped by school work; the cluster has mostly been sitting idle on a shelf collecting dust. However last weekend the project got revived. I made it a goal that I complete the project and document the path I take.

In the next post about the cluster, I will install an operating system onto the Pis and configure the network so that they can all communicate with each other. 
