---
title: "PHP: a warning message when a deprecated version is used" 
date: 2024-02-14
tags:
  - php
  - applications
  - information
authors:
  - name: David Legrand
    link: https://github.com/davlgd
    image: https://github.com/davlgd.png?size=40
description: Please, update!
excludeSearch: true
---

PHP ecosystem is evolving at a steady pace with a clear lifecycle: 1 version per year, 2 years of active support, plus 1 year of security support. Thus, PHP 8.2/8.3 are now the one actively supported, while 8.1 is in its security support window. ALL previous releases are considered end-of-life (EOL) by PHP Team, with no support. 

PHP 5.x branch is EOL since 2019, 7.x branch since the end of 2022. But we still see a lot of applications using them. So we start today to better inform our users about it. The first change they will notice is a warning during the application deployment if they use PHP 8.0 or a previous release, asking them to set `CC_PHP_VERSION` to `8` (latest 8.x), `8.2` or `8.3`.

In the coming months, we'll show such warnings in other interfaces and send emails about it. There is no short term plan to cut access to supported versions such as PHP 5.6 or 7.x, but you do it at your own risks.