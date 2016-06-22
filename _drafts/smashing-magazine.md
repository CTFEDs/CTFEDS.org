---
layout: page
title:
---

[Smashing Magazine](https://www.smashingmagazine.com/) is a well-known, long running, industry magazine that's evolved from listicles to in-depth articles over the years. A few years ago they did a big responsive redesign. We have a look at how it's doing in terms of Front-end performance.

## Statistics

* Google's PageSpeedInsight: [99/100 on mobile and desktop](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fwww.smashingmagazine.com%2F)
  * Webaim's WAVE: [2 errors and 65 alert](http://wave.webaim.org/report#/https://www.smashingmagazine.com/)
* WebPageTest on Motorola G, Chrome, 3G: [SpeedIndex of 4753, 4744 on repeat view](http://www.webpagetest.org/result/160622_JZ_b609c0546b8bd0d7807e8c259bac6d4a/)

## Review

Summary

- great results on PSI, WAVE, and WPT!
- lots of image requests, quite a lot of JS requests.
- Some weird external massive (0.5MB) CSS being loaded.

Generally speaking, the Smashing Magazine site is doing well on performance: they're even using Service Worker to cache a bunch of resources, which is great. It would be good to try and reduce the number of HTTP requests: about 54 images and 9 JS files. The images could be sprited and the JS files could be combined.


---

Published on ddd dd mmm yyy.

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
