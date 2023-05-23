---
layout: post
title:  "PrestaShop 8.1 Release Candidate Is Ready To Be Tested!"
subtitle: "After the Beta, the first release candidate for PrestaShop 8.1 is now ready for you to test!"
date: 2023-05-23
authors: [ PrestaShop ]
image: /assets/images/2023/02/banner_8.1_1200x627.jpg
twitter_image: /assets/images/2023/02/banner_8.1_1024x512.jpg
icon: icon-leaf
tags:
- version
- rc
- minor
- releases
- 8.1
---

We are happy to announce the first release candidate of PrestaShop 8.1.

![PrestaShop 8.1 Release Candidate 1 is available](/assets/images/2023/02/banner_8.1_1534x424.png)

We're on the brink of releasing the final 8.1 version. This time, the Release Candidate version is being shared simultaneously to the community and the project's Quality Assurance (QA) team. The idea is for everyone to collectively confirm that all issues identified in the beta version have been resolved, ensuring its suitability for production use. If no major problems are reported by June X, we'll move ahead and launch the final version of 8.1.

Remember, this version might still have some problems. So, it's not safe to use it in production environment yet! Also, please remember that ight now you can't move from the beta to the release candidate version, and you also can't move from this RC version to the final version using the upgrade module.

## Your feedback is important!

Much like the public beta, the release candidate phase holds great significance in gearing up for the forthcoming release. At this stage, we're urging all community members to get this version, install it, and see how it performs in their individual settings.

Here are some examples of how you can help:
* If you are a module or theme developer, check if they work well with this new version.
* If you notice any problem and you think it is caused by the new version, please [report it on GitHub](https://github.com/PrestaShop/PrestaShop/issues/new/choose).
* Don’t hesitate to [contribute to fixing bugs](https://devdocs.prestashop-project.org/8/contribute/contribute-pull-requests/) if you can!

**Your feedback is essential.** The more issues you report right now, the fewer bugs there will be on the final release, which means fewer patch versions and fewer problems on your (or your customer’s) online store.

**Please submit all your feedback by June X, 2023.** If no new critical or major issue remains to be fixed by then, the final release will be made available. This is the final chance to test this new version before the final release is out!

If you have any questions about the version and its features, feel free to share them on [the PrestaShop project’s Slack](https://www.prestashop-project.org/slack/).

And if everything is working well, feel free to comment on this article to tell us, and share your thoughts on social networks, we also need this kind of feedback! ;-)

## Notable changes since the beta release

- [Code related to the old product page has been deprecated and will be removed in PrestaShop 9.0](https://github.com/PrestaShop/PrestaShop/pull/32194)
- [New image management system is now under the "New feature" flag](https://github.com/PrestaShop/PrestaShop/pull/31662)
- [Some of the smarty functions are now registered manually, these changes may impact some of the third-party solutions](https://github.com/PrestaShop/PrestaShop/pull/32197)
- [Classic theme has been updated to version 2.1.1](https://github.com/PrestaShop/PrestaShop/pull/32574)

Other than that, there was a lot of changes regarding the new product page and other new features that are available in the 8.1 version.

Check out the [changelog](https://github.com/PrestaShop/PrestaShop/releases/tag/8.1.0-rc.1) to see all the changes in detail.

All the major bugs have been fixed, and [the remaining minor ones](https://github.com/PrestaShop/PrestaShop/issues?q=is%3Aopen+is%3Aissue+label%3A8.1.x+label%3ABug+label%3ARegression) will be fixed in the upcoming 8.1.1 patch release.

If you're curious about all the changes and new things coming in 8.1, the [8.1 beta version release note]({{< relref "/news/releases/prestashop-8-1-beta-release" >}}) is just the right thing for you to look at!

## Download

You can download PrestaShop 8.1 release candidate here:
[Download PrestaShop 8.1 release candidate now!](https://github.com/PrestaShop/PrestaShop/releases/tag/8.1.0-rc.1)

## Acknowledgments

A big thank you to the 36 people who contributed to this release candidate:

0x346e3730, Alexandre Hellin, Antonin Clauzier, bibips, Boris Hermans, Boubker Bribri, Cedric Vangout, Codencode, Daniel Hlavacek, Fabien Papet, Franck Lefèvre, Ibrahima Sow, Jakub Łach, Jens Wilke, jevgenijvisockij, Jonathan Lelievre, Julius Žukauskas, Krystian Podemski, Léa Delin, Lorenz Meyer, Mathias Reker, Mathieu Ferment, Matthieu Rolland, Maxime Flasquin, Nesrine Abdmouleh, Nicolas Lœuillet, Pablo Borowicz, PICHAT Morgan, Prestaworks, PrestonBot, Robin Fischer, Salim Benouamer, Sharak, Thomas Baccelli, Thomas Nares, Thomas Leone