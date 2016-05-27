---
layout: page
title: Mail and Guardian
---

We're starting a new series on CTFEDs: quick Friday lunchtime reviews of sites, with some suggestions for improvements.

## Statistics

* Google's PageSpeedInsight: [49 / 100 mobile, 14 / 100 desktop](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fmg.co.za%2F)
* Webaim's WAVE: [102 errors](http://wave.webaim.org/report#/http://mg.co.za/)
* WebPageTest on 3G: [SpeedIndex of 6830](http://www.webpagetest.org/result/160527_8C_b46fbe22acd0ce203f428c4d8d80a916/)

## Review

This week the [Mail & Guardian](http://mg.co.za/) launched a new website. Unfortunately there are a number of Front-end Performances issues. The biggest problems are:

- high number of http requests
- page size is huge
- load time is over a minute

They could dramatically improve the performance by **combining and concatenating CSS and JS files** thereby reducing the number of http requests. Even better would be to use fewer CSS files and JS files in the first place. There also appear to be unnecessary scripts - two versions of jQuery and a jQuery migration file that isn't applicable.

The biggest change they could make to improve page size is to **improve how they work with images**: there are nearly 100 images on the page. Looking at the PageSpeed results, optimising all the images on the page would save about 4MB. Better than that would be to serve smaller images to smaller screens, using `srcset` (with a small or medium image as the default in the `src` attribute). Even better than that would be having fewer images on the page, or lazy loading images further down.

Making the above improvements will greatly improve load times.

---

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
