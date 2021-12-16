---
layout: post
title:  "Backup, Migrate or Clone Wordpres Sites"
date:   2021-12-16 12:07:12 +0800
categories: wordpress backup migrate clone
---

This article will guide you on creating file for backup or for migrating or cloning a wordpress site.

Install [Backup Migration](https://wordpress.org/plugins/backup-backup/) by [Migrate]https://backupbliss.com/ which should be installed on both source and new site.
 
## Creating clone file

 1. Login to source site.
 1. Select **Backup Migration** on the Wordpress dashboard
 1. On the *Create backup()s* tab, click the large green button that says *Create Backup Now*. A popup will show and click the *Create the backup!*. A backup will process.
 1. After the backup is succesfully done, click **Copy** to copy the URL to be use on the new site.

## 2. Exporting clone file

 1. login to your new  site.
 1. Select **Backup Migration** on the Wordpress dashboard
 1.  On the *Manage and restore backup()s* tab, click *super quick migration* dropdown and paste the backup URL. Then click on the *Restore Now* Button
