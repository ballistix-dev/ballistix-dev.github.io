---
layout: post
title:  "Access Server with VPN"
date:   2018-11-02 08:17:00 +0800
categories: production vpn
---

1. Go and login to [https://34.199.38.17](https://34.199.38.17). (*Contact Kervin for your credentials*)

1. After login, download the **OpenVPN Connect app** according to your OS

   ![alt text]({{ "/assets/img/2018-11-02/download.png" | relative_url }})

1. Install downloaded file.

1. *Windows* - On notification bar, right click OpenVPN notification icon and go to 34.199.38.17 > Connect. Enter your credentials when asked. Server IP is 34.199.38.17. A success notification promt will show.

   ![alt text]({{ "/assets/img/2018-11-02/connect.png" | relative_url }})
   
1. To connect to CMS04, use host 10.0.1.220 
     
   - Terminal: `ssh username@10.0.1.220`
   - SFTP: Host: 10.0.1.220
