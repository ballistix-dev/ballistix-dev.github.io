---
layout: post
title:  "Allow permalinks on multi-wp, nginx"
date:   2019-07-18 07:36:12 +0800
categories: wordpress 
---

Go to /etc/nginx/sites-enabled

Edit 'test.ballistixwip.com.conf' 

add the sub site folder as 

    location /[NAME_OF_SITE_FOLDER] {
      index index.php index.html index.htm;
      try_files $uri $uri/ /[NAME_OF_SITE_FOLDER]/index.php?q=$uri&$args;
    }
    
Run terminal Restart server

    sudo /usr/sbin/service nginx restart
