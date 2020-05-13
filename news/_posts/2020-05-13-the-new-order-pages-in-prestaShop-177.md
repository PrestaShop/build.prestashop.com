---
layout: post
title: "The new order pages in PrestaShop 1.7.7"
subtitle: "Introducing the revamp of order pages"
date: 2020-05-13 9:00:00
authors: [MateusShirlaw]
icon: icon-lightning
tags:
- 1.7.7
- version
- minor
- product
- ux
---

With the release of the new version 1.7.7, this article has the ambition to detail one of the major features of the version. Our work was focused on one of the most used pages by our merchants: the orders' management page.

We are thrilled to introduce to you the new features around the order process. But before jumping into the features awaiting the merchants in the new version, we would like to share our thinking process.

**First, why rethinking this page in particular?**

The pages were becoming particularly unpleasant to use because of its old visual appearance and its hierarchy of information that led to inefficiency and misunderstanding for our merchants.

**A long process to ensure the full success of the revamp.**

To have a better understanding of the merchants' pain points, we have interviewed merchants with different sales volume, country and business activity as well as agencies of different sizes. The pain points encountered have then been addressed by the features added in the order list page (I) and order detail page (II).

**Now, let's present these changes.**

## I.  Concerning the page listing the orders, we have added the following features

**The listing order page's new features aim at helping merchants save time and increase their productivity.**

- **Order's preview**: Opens a panel just below the line of the order to preview the order's essential information.

![Order preview](/assets/images/2020/05/order_preview.gif "Order preview")

***What is the goal***:

Allows the merchant to check, prepare and track his order without having to open it. So the merchant won't have to open the order to check essential information that doesn't require actions.

***How it works***: 

When the user clicks on the icon, it displays the order's preview below the line selected. The order preview lists the following information: the invoice address, the shipping address, the customer details, the carrier details (and the tracking ID when available) and the products' list. 

The products' list displays on each line the product name, reference, stock location (if available), quantity, tax price and total price for the products. The total price follows the customer group configuration. If the customer group sets the prices with or without tax, it impacts the displayed amount in the total column and adds the related label "tax excluded" or "tax included".

The list displays the 10 first products. The remaining products can be seen by expanding the list.

There is a new hook called displayOrderPreview on the bottom of the preview.

![Order preview's hook](/assets/images/2020/05/hook-preview.png "Order preview's hook")

It allows modules to add new elements on the preview. For more specific needs, the preview can be changed by overriding templates, [find here](https://devdocs.prestashop.com/1.7/modules/concepts/templating/admin-views/) more information.


&nbsp;
- **Editable order status labels:** Allows to change the order status directly from the listing.
 
![Order page - Edit a status](/assets/images/2020/05/editable_order_statuses_labels.png "Edit a status")

***What is the goal***:

Making the order fulfillment less time consuming for the merchants

***How it works***: 

When the user clicks then on the status label, it displays a drop-down list with all of the available statuses. By selecting one of the items on the list, the user can update the order status.


&nbsp;
- **Statuses' color**: Color according to the order status

![Order statuses by category](/assets/images/2020/05/order_status_labelsx2.png "Order statuses by category")

***What is the goal***: 

The colors used by default to contextualize the status is based on a wide range of colors without following any real logic. To bring a structure and meaning to the statuses colors, the statuses are grouped in 4 colors categories:

- Dark blue: orders waiting for a customer action ( i.e. waiting for a bank check-in)
- Light blue: orders waiting for a merchant action following an accepted payment 
- Green: no action needed from the merchant (i.e. when the product is delivered)
- Red or black: special status (i.e. payment error)

The merchants have a concise view of the work remaining to be done between the order to be prepared and the delivered order.

***How it works***: 

The statuses color is set by default. They are still configurable in the Order Setting page.


&nbsp;
- **Link to the customer's profile**: Creates easy access to the customer's profile by clicking on its name.

![Right click on the customer's link](/assets/images/2020/05/link-customer.png "Right click on the customer's link")

***What is the goal***: 

Merchants used to have to open the order to get access to the customer page. It is now accessible from the orders listing.

***How it works***:

Clicking on the customer name opens the customer page in a new tab.


&nbsp;
- **Bulk action redesign** : The bulk actions' design and its position were updated to make it more visible and quicker to use.

![Change_order's statuses](/assets/images/2020/05/choose_an_order.png "Change_order's statuses")

***What is the goal***: 

To help the merchants to process multiple orders in 3 clicks.

***How it works:*** 

Select several orders, choose the new order status in the pop-in then validate it to update the orders' status.


&nbsp;
- **Open in new tabs**: Open commands in new tabs by mass action to process them as the merchant proceeds.

![Open in new tabs](/assets/images/2020/05/open_in_new_tabs.png)

***What is the goal***: 

If the merchant has a poor internet connection, he can now open orders in advance to them to load in the background. 

***How it works***: 

Choose several orders, select _open in new tabs option_ on bulk action's option to open them in new tabs.

## II. For the order details, we have added the following features:

Even if we keep the objective of saving time and productivity, the improvements and features are focused on readability and the position of the information. Indeed, some important information did not have the display corresponding to its importance. For example, the list of products that were at the bottom of the page is now at the top of the page as it is the first information to be consulted.

**Thus with better readability, we allow the merchant to be more efficient in his work.**


- **Pagination on the product list**: Allows to navigate in the order product list through the pagination.

![Order's_pagination](/assets/images/2020/05/order_pagination.png)

***What is the goal***:

Avoid an endless and unreadable list of products. Pagination provides structure in the products' navigation. Also, the list has been moved to the top of the page to avoid the merchant from scrolling to the bottom of the page to see the products ordered.

***How it works***:

The pagination of the list starts when there are more than 8 products in the cart. The stock location column is displayed when one of the products has a stock location. Also, It is only displayed at the corresponding pagination.


&nbsp;
- **Pack & customized products:** Display the product's customization on the list and gives access to a pack content through a pop-in.


***What is the goal***: 

Easy check and verification directly from the list.

***How it works***:

For customized products - files or texts are displayed below the product. The files are added in a new column on the same line. The texts are displayed below each other.

![Customized products](/assets/images/2020/05/custom-product.png)



Pack of products - A link bellow the products' pack displays the related products with the ordered quantity and the available product stock. 

![Pack of products](/assets/images/2020/05/pack-product.png)


&nbsp;
- **Message interface:** Display the 4 latest messages and allows the merchant to see the whole conservation in a pop-in.

![Order's messages](/assets/images/2020/05/messages-order.png)

***What is the goal***:

To ease the discussion readability through a modern interface, inspired by the current messaging apps. 

***How it works***: 

The differentiation between private messages has been reinforced. It is only visible to the merchant. This allows for better readability and reduces misunderstandings.
At the 5th message between a customer and the merchant, a link is displayed to open the pop-in which displays the entire conversation.


&nbsp;
- **Hooks**: New hooks positions.

![Order hooks mapping](/assets/images/2020/05/order_details_hooks.jpg "Order hooks mapping")

***What is the goal***: 

The hooks have been relocated to more strategic positions to match the layout redesign and thus provide a better user experience.

***How it works***: 

Find [here](https://devdocs.prestashop.com/1.7/modules/core-updates/1.7.7/) the documentation on the hooks' mapping. A new hook grouping the actions of the top of the order page has also been added to replace displayBackOfficeOrderActions which will no longer have the same layout.

The detailed changes can be found on the following pull requests on github [#16144](https://github.com/PrestaShop/PrestaShop/pull/16144) and [#17734](https://github.com/PrestaShop/PrestaShop/pull/17734).

A summary of the hooks impacted:

  - displayAdminOrderTop (alias of displayInvoice)
  - displayBackOfficeOrderActions
  - displayAdminOrderSide (replace displayAdminRight)
  - displayAdminOrderMain (replace displayAdminLeft)
  - displayAdminOrderTabLink (replace displayAdminOrderTabOrder et displayAdminOrderTabShip)
  - displayAdminOrderTabContent (replace displayAdminOrderContentOrder and displayAdminOrderContentShip)
  - actionGetAdminOrderButtons

Over the last few months, PrestaShop has been working hard to deliver these new features and many bugs fixes on these pages. 31 bugs, including 8 majors, 16 minors and 3 trivials, have been fixed from the previous 1.7 and 1.6 versions. For more information, you can find [the way we classified the severity of the bug](https://build.prestashop.com/news/severity-classification/) and [the list of the fixed bugs](https://github.com/PrestaShop/PrestaShop/issues?q=is%3Aissue+label%3AOrder+milestone%3A1.7.7.0+label%3ABug+-label%3ARegression+sort%3Acreated-asc+is%3Aclosed). Overall, the order project has ensured more stability by correcting ⅔ of the major bugs of the order page.

We encourage you to try out the features on the beta version and share any feedback [here](https://github.com/PrestaShop/PrestaShop/issues/new/choose). Your opinion is important to us. We are counting on you to share your feedback and new ideas with us so that we can continue to develop the PrestaShop that you need.

We would like to thank WebXY, YATEO, Ecomiz and VAISONET and all the merchants interviewed for taking the time to exchange with us.
