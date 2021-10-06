---
layout: post
title: PrestaShop 1.7.8.0 is available
subtitle: You waited for it, here it is!
date:  2021-10-05
authors: [PrestaShop]
image: /assets/images/2021/10/1780_banner_1200_628.jpg
icon: icon-leaf
tags:
 - version
 - 1.7
 - 1.7.8.x
 - minor
 - releases
---

We are happy to announce PrestaShop 1.7.8.0 is officially available!

![1.7.8.0 is available!](/assets/images/2021/10/1780_banner_1200_628.jpg)

Each version of PrestaShop is getting bigger and bigger, with more and more regular contributors. We are very proud of having such a strong community working with us on a daily basis.

This new version brings many features that should please both merchants and developers. 

# New in 1.7.8.0
## Support PHP 7.4

This version is compatible with PHP 7.4. it is allows the software to have access to the latest bug fixes and security vulnerabilities from PHP. 
NB: PHP 7.3 no longer provides support except for security fixes until January 2022. Find more information [here](https://devdocs.prestashop.com/1.7/basics/installation/system-requirements/).

## New translations features

![illustration translation](/assets/images/2021/10/illustration_translation.png)

* It is now possible to export back-office, front-office, email, themes, and module translations.
* Modules using the  [new translation system](https://devdocs.prestashop.com/1.7/modules/creation/module-translation/new-system/)  introduced in 1.7.6 can now distribute their own translation files in the XLF format. Users can use the export tool to migrate from legacy PHP catalogue to XLF catalogue
Developers have better translation system to manage the translations of their modules or themes.

##  New multistore header

![illustration multistore](/assets/images/2021/10/illustration_multistore.png)
 
You can search search shop and personalized on the multistore header. The new header offers a brand new multistore experience for the merchants.
[Here to see the detail of the feature](https://build.prestashop.com/news/multistore-news-in-1.7.8/) 

## The implementation of Native Lazy Loading on theme Classic

![illustration lazy loading](/assets/images/2021/10/illustration_lazy_loading.png)

Lazy loading is a technique that defers the loading of non-critical resources to the page load. We recommend all theme developers to this technology to enhance their themes to improve the merchant’s store performances.

## Improvement of the UI

![illustration ui kit](/assets/images/2021/10/illustration_ui_kit.png)

PrestaShop back-office UI Kit has been improved to have a solid Design System with adjustment of alert colors, font size, buttons contrasts, and an enhancement of the responsiveness.

**IMPORTANT NOTE** if you plan on upgrading your shop to 1.7.8 and your current version is **below 1.7.6** you need to use the latest version (4.11.0) of our [1-Click Upgrade module](https://github.com/PrestaShop/autoupgrade). Of course, it’s always recommended using the latest version when upgrading, but even more so in this case since a bug related to upgrading from these older versions has been fixed in the module.

## And many more features and improvements
If you are looking for more details about all changes and new features expected in 1.7.8, the [1.7.8 beta version release note](https://build.prestashop.com/news/prestashop-1-7-8-0-beta-release/) is the perfect article for you to read!

## Notable fixes since RC1
The RC allowed a member of the community to detect a bug on the CLI. 
This major bug [#25982](https://github.com/PrestaShop/PrestaShop/issues/25959) blocked the installation of a PrestaShop from the CLI. 

## Changelog

1 492 pull requests have been merged since the beginning of the version development. Read the [Changelog](https://github.com/PrestaShop/PrestaShop/releases/tag/1.7.8.0) for details. 

// add data between releases

## Download

You can download PrestaShop 1.7.8.0 here:

[Download PrestaShop 1.7.8.0 now!](https://www.prestashop.com/en/developers-versions){: .btn .btn-lg .btn-success}
{: .text-center}
 
PrestaShop 1.7.8.0 is also available through the 1-Click Upgrade module. 

## Known issues

All the major bugs have been fixed, and [the remaining minor ones](https://github.com/PrestaShop/PrestaShop/issues?q=+is%3Aissue+milestone%3A1.7.8.1+) will be fixed in the upcoming 1.7.8.1 patch release.

## Acknowledgments

PrestaShop is above all a community project: from the 119 committers who contributed to this release, the vast majority are not directly affiliated with the PrestaShop company. Also, 57 people contributed for their first time to PrestaShop in this version!

All contributors:
//add list

A huge thanks to everyone involved in this version!
Thank you again for helping improve the lives of more than 300,000 online merchants with ideas, improvements, and fixes!
