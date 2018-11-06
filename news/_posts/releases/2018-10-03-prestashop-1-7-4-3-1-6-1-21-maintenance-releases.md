---
layout: post
title:  "Release of PrestaShop 1.7.4.4 and 1.6.1.23"
subtitle: "Maintenance version of the 1.7.4.x and 1.6.1.x branch"
date:   2018-11-06 18:00:00
authors: [ AntoineThomas ]
icon: icon-leaf
tags:
 - version
 - maintenance
 - patch
 - releases
 - 1.7.4.x
 - 1.7
 - 1.6.1.x
 - 1.6
---

PrestaShop 1.7.4.4 and 1.6.1.23 are now available. These versions fix a security issue for both 1.7.4.x and 1.6.1.x. For the details, please read below:

These two security updates fix some issues on the filemanager integrated in TinyMCE in the back office. The use of three security issues allowed, for a user with BO access, to upload some malicious hidden Phar files that would then allow to execute some code on server side and get back the result.

Since these versions fix security problems, we **strongly** encourage you to upgrade your shop as soon as possible.

Changes for 1.7.4.4 and 1.6.1.23 are:

- Core:
  - Bug fix:
    - Remove filemanager action image_size
    - Check mime type when uploading files
    - Fixed arbitrary image write/overwrite in Windows installation
    - Prevent image directory deletion

[Complete list of changes for 1.7.4.4](https://github.com/PrestaShop/PrestaShop/releases/tag/1.7.4.4)

[Complete list of changes for 1.6.1.23](https://github.com/PrestaShop/PrestaShop/releases/tag/1.6.1.23)

[Download PrestaShop now!](https://www.prestashop.com/en/download){: .btn .btn-lg .btn-success}
{: .text-center}


Contributors to this patch versions, from both the Core team and the community at large: 
Thank you! Three of you contributed for the very first time, warm welcome :-)

A very special thank to Fariskhi Vidyan (@farisv) for the security reports, and his help during our correction of these issues!

Since version 1.7.4.4 is a "patch" update to version 1.7.4.3, upgrading from any 1.7.4 version will be easy: features will work better, and modules & themes which worked fine on 1.7.4.x will work just as well with 1.7.4.4.<br/>
Upgrades from a standard 1.7.x version should work just as well.

This the same for 1.6.1.23 regarding 1.6.1.x versions.
