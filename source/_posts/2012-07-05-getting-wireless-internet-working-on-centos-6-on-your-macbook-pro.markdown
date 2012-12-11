---
layout: post
title: "Getting Wireless Internet Working on Centos 6 on your MacBook Pro"
date: 2012-07-05 12:00
comments: true
categories: centos macbookpro networking wireless
---
At home I have been setting up CentOS 6.2 on a spare MacBook Pro (thanks to my IS friend at work) for learning about RHEL 6.  Since I use a wireless router, I wanted to get a wireless connection setup on the laptop.  The MacBook Pros use a Broadcom wireless NIC:
```
$ lspci | grep Broadcom
04:00.0 Network controller: Broadcom Corporation BCM43224 802.11a/b/g/n Wireless LAN Controller (rev 01)
```
I initially tried compiling and installing the Broadcom driver following the (roughly similar) steps described [here](http://ktaraghi.blogspot.com.au/2011/08/how-to-install-broadcom-bcm4311-bcm4312.html) and [here](http://wiki.centos.org/HowTos/Laptops/Wireless/Broadcom) but with no luck (#sadtrombone).

Later, I saw a note at the top of the second page (referenced above) which linked to a source RPM called [wl-kmod](http://elrepo.org/tiki/wl-kmod) on [ELRepo.org](http://elrepo.org/).  I thought I'd give it one more try so I followed the relatively short and simple instructions on the wl-kmod page and it worked without a hitch!

The steps involve you installing some development tool packages, downloading a SRPM for wl-kmod, downloading the source for the Broadcom driver (64-bit in my case), building and installing the final RPM for wl-kmod.  Once you either reboot or manually add the Linux kernal modules from the command line you see a new "Wireless Networks" section appear under the already existing "Wired Networks" section on the top right of your desktop (if you are running one that is).

You can then proceed to select one of the wireless networks that are detected (or manually add one yourself) and enter the wireless security details.

From the command line you will see the new wireless interface:
```
$ ifconfig eth1
eth1    Link encap:Ethernet HWaddr:xxxxxxxxxxxx
        inet addr:xxxxxxxxxx
        ...etc...
```
From then onwards it should just work!
