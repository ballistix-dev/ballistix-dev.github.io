---
layout: post
title:  "Use Host Switch"
date:   2018-10-22 07:38:12 +0800
categories: wordpress staging
---

Host Switching is needed when we want to test an instance, and want to use the production URL which is being currently used by another instance. Some reasons of this is to maintain the URL links of assets and settings.

There are a couple of ways do host switch, but basically you first needed to first know the IP address of the host you are going to switch to and the domain of the site.

    52.5.15.126 www.whitehatvirtual.com

### via Google Chrome extension

1. Install an extension on your Google Chrome called [Host Switch Plus](https://chrome.google.com/webstore/detail/host-switch-plus/bopepoejgapmihklfepohbilpkcdoaeo)
1. Open the extension on the browser taskbar and click Add.
1. Enter the IP and Domain and click Submit.
1. You need to open the extension again and click on the gray circle before the newly added entry to activate it.
1. Go to the URL.

### use an Application

1. Go to [SwitchHosts git](https://github.com/oldj/SwitchHosts) and [download](https://github.com/oldj/SwitchHosts/archive/master.zip) latest repo.
1. Extract files and run as administrator 'SwitchHosts!'
1. add IP and domain
1. Go to the URL.
