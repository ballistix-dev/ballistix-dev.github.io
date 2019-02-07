---
layout: post
title:  "using-invisible-recaptcha-on-mautic-for-wordpress"
date:   2019-02-06 07:36:12 +0800
categories: wordpress mautic wordpress
---

 1. Follow this instruction to install and activate reCaptcha on Mautic Instance https://github.com/KonstantinCodes/mautic-recaptcha
 1. on the form's submit button, add this to the input attributes
    class="btn btn-default g-recaptcha" data-sitekey="6Lc4cY8UAAAAAA_sAwNa4zRQqEkqSqylGmGm8yP4" data-callback='onSubmit'
 1. before the shortcaode on wordpress
     
     <script src="https://www.google.com/recaptcha/api.js" async defer></script>
     <script>
       function onSubmit(token) {
         document.getElementById("mauticform_webcontactform").submit();
       }
     </script>
