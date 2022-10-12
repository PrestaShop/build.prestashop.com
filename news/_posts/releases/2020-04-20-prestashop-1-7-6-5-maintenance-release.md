---
layout: post
title:  "Release Of PrestaShop 1.7.6.5"
subtitle: "Maintenance version of the 1.7.6.X branch"
date:   2020-04-20 16:30:00
authors: [ PrestaShop ]
image: /assets/images/2020/04/1765meta.jpg
icon: icon-checked
tags:
 - 1.7
 - 1.7.6.x
 - version
 - patch
 - releases
 - security
redirect_from:
 - /news/release-note-1765/
---


A few months ago, the PrestaShop core team has decided to make a forthright patch release process and deliver patch versions on a more regular basis, every time it’s needed. So here we are, 6 weeks after the release of 1.7.6.4, PrestaShop 1.7.6.5 is now available! 

![1.7.6.5 is available!](/assets/images/2020/04/1765banner.jpg)

This maintenance release is a bit special as it does not only fix regressions found on version 1.7.6.0 to 1.7.6.4, but it also has put a focus on fixing many security issues, from 1.5, 1.6 and 1.7 versions. This is a result of a huge work on security which has been started a few weeks ago to ensure more security on the PrestaShop software. In the near future, PrestaShop will focus more and more on security to ensure that no security breaches, even minor ones such as permission issues, are left out in the core. 

As this patch fixes several security issues, we highly recommend to upgrade your shop as soon as possible. Of course, as always, don’t forget to backup before.

Reminder:  the 1-Click Upgrade module’s latest version is [v4.10.1](https://github.com/PrestaShop/autoupgrade/releases/tag/v4.10.1), don’t forget to upgrade it.


## Main fixes

Below are listed the 7 regressions that were found and fixed in this version, impacting both front-office and back-office.

Front-office regressions:

- When editing an address both in the customer account and checkout, a new address was created instead of replacing it - [#18100](https://github.com/PrestaShop/PrestaShop/issues/18100) and [#18072](https://github.com/PrestaShop/PrestaShop/issues/18072)
- Canonical redirects for products with combinations no longer worked, which could cause duplicate content [#18279](https://github.com/PrestaShop/PrestaShop/issues/18279)

Back-office regressions:

- When adding a cart rule to an order from the back-office, the value discount was not correct [#18630](https://github.com/PrestaShop/PrestaShop/issues/18630)
- Searching a category with the quick search no longer redirected to the category edition page - [#17908](https://github.com/PrestaShop/PrestaShop/issues/17908)
- The help card was no longer displayed on view order and new employee pages - [#18279](https://github.com/PrestaShop/PrestaShop/issues/18279) and [#18615](https://github.com/PrestaShop/PrestaShop/issues/18615)
- In the customer view page, the number of “last emails” was incorrect - [#18602](https://github.com/PrestaShop/PrestaShop/issues/18602)
- It was not possible to access the translation interface for the Serbian language - [#18062](https://github.com/PrestaShop/PrestaShop/issues/18062)


## Security fixes

Some security fixes have been included in this patch version to ensure an improved core reliability. Thanks a lot to Rabhi for finding a lot of these issues !

Improper access controls:

- on product page with combinations, attachments and specific prices ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-cvjj-grfv-f56w))
- on product attributes page ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-4wxg-33h3-3w5r))
- on customers search ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-r6rp-6gv6-r9hq))
- on several other pages ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-74vp-ww64-w2gm))

Reflected XSS:

- related in import page ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-98j8-hvjv-x47j))
- with back parameter ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-j3r6-33hf-m8wh))
- on Exception page ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-mrpj-67mq-3fr5))
- on AdminCarts page ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-q6pr-42v5-v97q))
- on Search page ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-rpg3-f23r-jmqv))
- on dashboard calendar ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-m2x6-c2c6-pjrx))
- on AdminFeatures page ([security advisor](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-87jh-7xpg-6v93))
- on AdminAttributesGroups page ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-7fmr-5vcc-329j))
- in security compromised page ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-48vj-vvr6-jj4f))

Open redirection:

- with the back parameter ([security advisory](https://github.com/PrestaShop/PrestaShop/security/advisories/GHSA-375w-q56h-h7qc))

A few security issues have also been fixed on native modules:

- Faceted Search - Reflected XSS with url_name parameter ([security advisory](https://github.com/PrestaShop/ps_facetedsearch/security/advisories/GHSA-mmmv-m5q9-g3cm)) 
- Social follow - Reflected XSS with social networks fields ([security advisory](https://github.com/PrestaShop/ps_socialfollow/security/advisories/GHSA-774w-fg8p-7c8w))
- Link List - Stored XSS on back office edit page ([security advisory](https://github.com/PrestaShop/ps_linklist/security/advisories/GHSA-vr7g-vqp5-966j)) and stored XSS with custom URLs  ([security advisory](https://github.com/PrestaShop/ps_linklist/security/advisories/GHSA-cx2r-mf6x-55rx)) 

More information about why it’s important to update:

- [Improper Access Control](https://cwe.mitre.org/data/definitions/284.html)
- [Cross-site Scripting (XSS)](https://cwe.mitre.org/data/definitions/79.html)
- [Open Redirect (CWE-601)](https://cwe.mitre.org/data/definitions/601.html)


## Other main changes 

Improved installation under CLI by adding the “rewrite” parameter in “index_cli.php” to enable the rewrite engine (Pull request [#18491](https://github.com/PrestaShop/PrestaShop/pull/18491)).

Read the [full changelog here](https://www.prestashop.com/en/release-notes-1-7-6-5-stable).

## Acknowledgments

Contributors to this patch version, from both the Core team and the community at large: 
Franck Lefèvre, Ibrahima Sow, Jonathan Lelievre, Louise Bonnard, Matthieu Rolland, Pablo Borowicz, Pierre Rambaud, PululuK.
Thank you!


[Download PrestaShop 1.7.6.5 now!](https://www.prestashop.com/versions){: .btn .btn-lg .btn-success}
{: .text-center}



Since version 1.7.6.5 is a “patch” update to version 1.7.6.4, upgrading from any 1.7.6 version will be easy: features will work better, and modules & themes which worked fine on 1.7.6.x will work just as well with 1.7.6.5. Upgrades from a standard 1.7.x version should work just as well.
