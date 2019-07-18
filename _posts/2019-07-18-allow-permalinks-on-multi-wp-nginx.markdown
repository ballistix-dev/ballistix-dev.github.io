---
layout: post
title:  "Allow permalinks on multi-wp, nginx"
date:   2019-07-18 07:36:12 +0800
categories: wordpress 
---

1. Go to /etc/nginx/sites-enabled

1. Edit 'test.ballistixwip.com.conf' 

1. add the sub site folder as 

    location /[NAME_OF_SITE_FOLDER] {
      index index.php index.html index.htm;
      try_files $uri $uri/ /[NAME_OF_SITE_FOLDER]/index.php?q=$uri&$args;
    }
    
1. Run terminal Restart server

    sudo /usr/sbin/service nginx restart
