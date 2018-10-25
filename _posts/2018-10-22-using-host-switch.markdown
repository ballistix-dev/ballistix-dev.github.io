---
layout: post
title:  "Use Host Switch"
date:   2018-10-22 07:38:12 +0800
categories: wordpress staging
---

Host Switching is needed when we want to test an instance, and want to use the production URL which is being currently used by another instance. Some reasons of this is to maintain the URL links of assets and settings.

Basically you first needed to first know the IP address of the host you are going to switch to and the domain of the site.

    52.5.15.126 www.whitehatvirtual.com

### use an Application

1. Go to https://github.com/oldj/SwitchHosts/releases and select/download the release depending on your OS.
1. Extract files and run as administrator **SwitchHosts!.exe**
1. add IP and domain
1. Go to the URL.
