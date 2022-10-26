---
author: "Sam McLeod"

readingTime: true
categories: tech
date: "2016-05-23T00:00:00Z"
#description:Monitoring SystemD Units With Nagios
image: feature-laptop.jpg
tags:
- tech
- software
title: Monitoring SystemD Units With Nagios
---


_Ever forgotten to add a critical service to monitoring?_

_Want to know if a service or process fails without explicitly monitoring every service on a host?_

...Then why not use SystemD's existing knowledge of all the enabled services? Thanks to 'Kbyte' who made a simple Nagios plugin to do just this!

Screenshot:

![](http://kbyte.snowpenguin.org/portal/wp-content/uploads/2014/11/nagios.png)
<!--more-->

Requirements:

- Python3 (For RHEL/CentOS 7 `yum install python34`)
- python-nagiosplugin [My pre-built RPMs](https://packagecloud.io/app/s_mcleod/centos7/search?q=python-nagiosplugin) or `pip3 install nagiosplugin`
- [PyNagSystemD](https://github.com/kbytesys/pynagsystemd/blob/master/bin/pynagsystemd.py)
