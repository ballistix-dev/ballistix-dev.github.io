---
layout: post
title:  "Configure Cloudflare"
date:   2021-02-16 07:36:12 +0800
categories: production dns
---



![alt text]({{ "assets/img/cloudflare.png" | relative_url }} "Step 1")

 1. Click on the DNS tab, then click "+ Add Record Button"

  Name/Host/Alias | Time to Live (TTL) | Record Type | Value / Answer / Destination
  --- | --- | --- | ---
  @ (can be blank)| 86400 | A | 3.232.12.224
  www | 86400 | A | 3.232.12.224

![alt text]({{ "assets/img/cloudflare-nameserver.png" | relative_url }} "Step 2")

 2. Below the list of Records, look for "Cloudflare nameservers", copy the NS records and create NS records on your DNS hosting.

