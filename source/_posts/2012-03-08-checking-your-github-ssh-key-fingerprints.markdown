---
layout: post
title: "Checking your GitHub SSH Key Fingerprints"
date: 2012-03-08 12:00
comments: true
categories:
---
Regular GitHub users are probably aware of the recent GitHub [security vulnerability](https://github.com/blog/1068-public-key-security-vulnerability-and-mitigation) that was exploited by this [fellow](http://homakov.blogspot.com.au/2012/03/im-disappoint-github.html). You've also probably just received instructions via email to [audit](https://github.com/settings/ssh/audit) your SSH keys.  An easy way to do this is to run following command on your SSH key(s) stored on your computer:
```
ssh-keygen -lf <path_to_your_public_ssh_key>
```
This will then display the fingerprint of your public key which you can then compare to fingerprint displayed next to your public key on GitHub.

Example:
```
ssh-keygen -lf dummy.pub  2048 d3:c7:8d:73:b4:6e:00:5d:ce:c6:85:04:9e:6c:67:51 dummy.pub (RSA)
```
In this case, the fingerprint is the part:
```
d3:c7:8d:73:b4:6e:00:5d:ce:c6:85:04:9e:6c:67:51
```
