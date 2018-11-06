---
layout: post
title:  "Configure NGINX for wordpress permalinks"
date:   2018-11-02 08:17:00 +0800
categories: staging nginx permalinks
---

To configure NGINX for wordpress permalinks.

edit test.ballistixwip.com.conf

      $  sudo vi /etc/nginx/site-enabled/test.ballistixwip.com.conf

Edit/add/append the following location block within the server block:

      location / {
            try_files $uri $uri/ /index.php?$args;
      }

      ### if in sub directory

      location /[subdirectoryname] {
        index index.php index.html index.htm;
        try_files $uri $uri/ /[subdirectoryname]/index.php?q=$uri&$args;
      }

Save and close the file. Restart/reload your nginx server, run:

      sudo /usr/sbin/service nginx restart

in wordpress CMS, In the Settings > Permalinks panel, you can choose one of the more common permalink structures.
