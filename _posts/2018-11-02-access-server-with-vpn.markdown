---
layout: post
title:  "Access Server with VPN"
date:   2018-11-02 08:17:00 +0800
categories: production vpn
---

### Setting VPN

1. Go and login to <a href="https://34.199.38.17/?src=connect" target="_blank">https://34.199.38.17/?src=connect</a>. 

1. After login, download the **OpenVPN Connect app** according to your OS

   ![alt text]({{ "/assets/img/2018-11-02/download.png" | relative_url }})

1. Install downloaded file.

1. *Windows* - On notification bar, right click OpenVPN notification icon and go to 34.199.38.17 > Connect. Enter your credentials when asked. Server IP is 34.199.38.17. A success notification promt will show.

   ![alt text]({{ "/assets/img/2018-11-02/connect.png" | relative_url }})
   
### Connect to server

#### FTP

##### static.ballistixmail.com

1. Download and install [Filezilla](https://filezilla-project.org/download.php?type=client)
1. Open File > Site Manager
1. Click *New Site* and enter this details
   - Protocol: SFTP
   - Host: 10.0.1.220
   - Port: 22
   - Logon Type: Normal
   - User: your static.ballistixmail.com username
   - Password: your static.ballistixmail.com username
