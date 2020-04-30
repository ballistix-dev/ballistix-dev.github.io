---
layout: post
title:  "Cloning Wordpress Site using WP Clone"
date:   2020-03-31 07:36:12 +0800
categories: wordpress clone
---
## Prerequisite
 - [WP Clone](https://wordpress.org/plugins/wp-clone-by-wp-academy/) - should be installed on both source/staging and production site.
 
## Creating clone file
 
 ![alt text]({{ "assets/img/wp-clone-01a.jpg" | relative_url }} "Step 1")
 
 1. Login to source/staging site.
 1. Select **WP Clone** on the wordpress dashboard
 1. Make sure the *Create Button radio* is chosen then Click **Create Backup** button
 1. After the clone is done, click **Copy URL** beside the newly created clone.

## Exporting clone file
 
 ![alt text]({{ "assets/img/wp-clone-01b.jpg" | relative_url }} "Step 2")
 
 1. login to your new production site.
 1. Select **WP Clone** on the wordpress dashboard
 1. On **Restore from URL:** field, paste URL copied from staging
 1. Make sure the *Restore from URL radio* is chosen then Click on **Restore from URL:** to start process
