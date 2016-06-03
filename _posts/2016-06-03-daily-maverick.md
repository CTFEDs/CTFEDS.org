---
layout: page
title:
---

Intro blurb.

## Statistics

* Google's PageSpeedInsight: [46 / 100 mobile, 54 / 100 desktop](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fwww.dailymaverick.co.za%2F)
* Webaim's WAVE: [7 errors / 627 alerts](http://wave.webaim.org/report#/thedailymaverick.co.za)
* WebPageTest on 3G: [SpeedIndex of 12487](http://www.webpagetest.org/result/160601_AX_111H/)

## Review

The Daily Maverick is, in its own words, "a unique blend of news, information, analysis and opinion delivered from our newsroom in Johannesburg, South Africa". Their website unfortunately has a number of performance issues. These can be summarised as:

- large page size
- high number of http requests
- external scripts
- minimal caching
- css and js not minified
- images not compressed

Total page size for the home page is 4.4mb. The biggest factor affecting page size is javascript that weighs in at 2.7mbs. A large percentage of these come from third party domains again increasing time to load. A number of scripts are loaded at the top of the page. These can be moved to the bottom to minimise render blocking.

The home page currently has a very high number of requests at 247. 174 of them are images. While image size is generally small this still amounts to over 1mb of images and far too many requests. The design could be re-evaluated in this area. For example, does every story need to have an image attached to it? In many cases text will be sufficient to convey meaning. Where possible css and js files should be concatenated to minimise requests.

The large number of external scripts could be evaluated as to whether they are necessary or add value. For example, sharing scripts from third party services like Addthis add significant js size, requests and round trips to an external server. Considering that very few people engage with social sharing buttons (see [What Percent of Page Views Share on Social Media?](http://www.lukew.com/ff/entry.asp?1852)) these can either be removed or replaced with simpler versions (see [Ridiculously Responsive Social Sharing Buttons](http://kurtnoble.com/labs/rrssb/)).

Cacheable resources like css files, js files and images are not cached. Caching these will save network requests.

CSS and js files can be minified to save download time and images can be compressed to save foile size.

Making the above improvements will greatly improve load times.

---

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
