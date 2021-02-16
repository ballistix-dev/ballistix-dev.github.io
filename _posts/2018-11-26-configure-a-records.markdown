---
layout: post
title:  "Configure A Record"
date:   2018-11-26 07:36:12 +0800
categories: production dns
---

 1. Sign in to your domain's account at your domain host. [Who is my domain host?](https://whois.icann.org/en/lookup)
 1. Locate the page for updating your domain's DNS records.
 1. The page might be called something like DNS Management, Name Server Management, or Advanced Settings.
 
 if you are using Cloudflare, go to your site and click on the DNS tab, then click "+ Add Record Button"
 
 ![alt text]({{ "assets/img/cloudflare.jpg" | relative_url }} "Step 1")
 

    Name/Host/Alias | Time to Live (TTL) | Record Type | Value / Answer / Destination
    --- | --- | --- | ---
    Blank or @ | 86400 | A | 3.232.12.224
    www | 86400 | A | 3.232.12.224


 1. Save your changes and wait until they take effect.
