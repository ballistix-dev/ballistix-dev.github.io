---
layout: post
title:  "Setting up new wordpress project"
date:   2019-09-26 07:36:12 +0800
categories: wordpress vvv staging
---

### Requisite for local development

 1. [vvv](https://varyingvagrantvagrants.org/). For [installation instructions](https://varyingvagrantvagrants.org/docs/en-US/installation/software-requirements/)
 
### Deploying local site

 1. add this on `vvv-custom.yml`. Change instances of 'mysite' to project name.
 
        mysite: # vagrant provision --provision-with site-mysite
          repo: https://github.com/ballistix-dev/custom-site-template.git
          custom:
            # locale: it_IT
            delete_default_plugins: true
            install_plugins:
              - siteorigin-panels
              - so-widgets-bundle
              - https://github.com/marcelbaduaballistix/ballistix-so-bundle/archive/master.zip
              - https://github.com/marcelbaduaballistix/animated-classes/archive/master.zip
          hosts:
            - mysite.test
  
  2. Run provision `vagrant provision --provision-with site-mysite`
