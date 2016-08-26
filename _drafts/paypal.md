---
layout: page
title: PayPal
---

[Paypal](http://paypal.com) is a service used by millions of people around the world to do pay and get paid online. Available in 202 countries and 25 languages they are the de facto solution for online transactions. Their home page is largely a product showcase, designed to encourage users to sign up. We have a look at how they are doing in terms of Front-end performance.

## Statistics

* Google's PageSpeedInsight: [63/100 mobile, 74/100 desktop](https://developers.google.com/speed/pagespeed/insights/?url=paypal.com)
* WebPageTest on 3G: [SpeedIndex of 11168, 3975 on repeat view]()

## Review

The Paypal site does fairly well on performance measures but there is definite room for improvement.

- Page size is relatively high at just over 2mb and there are 37 requests. Images could be optimised to reduce file size and the autoplaying video in the header could be reconsidered as it offers little value to the user.
- There are 6 js files and 3 css files. These could be combined to save on requests. They are also not minified which increases their size significantly.
- Perhaps most surprising is the fact that the Paypal website is not responsive. Instead it appears that they are device sniffing in order to serve different layouts to devices.

The biggest improvement Paypal can make would be to **minimise requests** by combining CSS and js files, **minifying** CSS and js files, **optimising** images and considering the image of the autoplaying video.

Something about browser sniffing.

---

Published on ddd dd mmm yyy.

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
