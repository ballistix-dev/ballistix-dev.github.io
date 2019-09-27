---
layout: post
title:  "Setting up new wordpress project"
date:   2019-09-26 07:36:12 +0800
categories: wordpress vvv staging
---

### Requisite for local development

 1. [varyingvagrantvagrants(vvv)](https://varyingvagrantvagrants.org/). For [installation instructions](https://varyingvagrantvagrants.org/docs/en-US/installation/software-requirements/)
 
### Deploying local site

 1. add this on `vvv-custom.yml`. Change instances of *mysite* to project name.
 
        mysite: # vagrant provision --provision-with site-mysite
          repo: https://github.com/ballistix-dev/custom-site-template.git
          hosts:
            - mysite.test
          custom:
            delete_default_plugins: true
            install_plugins:
              - siteorigin-panels
              - so-widgets-bundle
              - https://github.com/marcelbaduaballistix/ballistix-so-bundle/archive/master.zip
              - https://github.com/marcelbaduaballistix/animated-classes/archive/master.zip
            wpconfig_constants:
              WP_DEBUG: true
              WP_DEBUG_LOG: true
              DISALLOW_FILE_EDIT: true
              WP_DISABLE_FATAL_ERROR_HANDLER: true # To disable in WP 5.2 the FER mode
          
  
  1. On terminal, go to your vvv folder and run this command `vagrant provision --provision-with site-mysite` remember to change *mysite* to project name. this will install the latest wordpress, necessary plugins, and custom themes. A user is already been setup (check terminal for credentials). 

### About Themes and Plugins pre-installed

#### Themes

 1. **_dash:**_ mother theme for theming. 
 1. **_ballistix:**_ child theme for theming. Utilizes Gulp for automated compiling of styles and scripts. Run `gulp serve`.
 
 #### Plugins
 
 1. **ballistix-so-bundle:** includes customized widgets. Dont Forget to activate widget under **Plugins** > **SiteOrigin Widgets**
    - Accordion Widget
    - Tabs Widget
    - Responsive Menu Widget
 1. **animated-classes:** animates an element by adding data attribute `data-animate="[animation-type]"`. For list of animation, refer to [Animate.css](https://daneden.github.io/animate.css/).
 
