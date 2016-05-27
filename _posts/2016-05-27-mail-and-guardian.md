---
layout: default
title: Mail and Guardian
---

We're starting a new series on CTFEDs: quick Friday lunchtime reviews of sites, with some suggestions for improvements.

## Statistics

* Google's PageSpeedInsight: [49 / 100](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fmg.co.za%2F).
* Webaim's WAVE: [102 errors](http://wave.webaim.org/report#/http://mg.co.za/)
* WebPageTest on 3G: [SpeedIndex of ](http://www.webpagetest.org/result/160527_8C_b46fbe22acd0ce203f428c4d8d80a916/)

## Review

The new [Mail & Guardian site](http://mg.co.za/) has a number of Front-end Performances issues. There are a lot of HTTP requests, the total size of the home page is about 10MB, and it takes over a minute to completely load the page.

The biggest change they could make is to **improve how they work with images**: there are nearly 100 images on the page. Looking at the PageSpeed results, optimising all the images on the page would save about 0.5MB. Better than that would be to serve smaller images to smaller screens, using `srcset` (with a small or medium image as the default in the `src` attribute). Even better than that would be having fewer images on the page, or lazy loading images further down.

Another thing that would improve the performance in **combining and concatenating CSS files** and **combining and concatenating JS files**. Better than that would be to use fewer CSS files and JS files in the first place. It looks like there are two version of jQuery and a jQuery migration file that isn't applicable

---

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
