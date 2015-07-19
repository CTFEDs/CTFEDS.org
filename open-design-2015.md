# CTFEDs event at Open Design Cape Town

## Principles

For Front-end developers, **Design is for Tomorrow** means embracing two "big ideas": being Future Friendly, and using Progressive Enhancement.

### Future Friendly

Future Friendly is a way of thinking that admits that we don't know what's coming next. It's about broad design principles and future-friendly values rather specific techniques.

> The quantity and diversity of connected devices - many of which we haven't imagined yet—will explode, as will the quantity and diversity of the people around the world who use them.

It's about choosing to:

* Acknowledge and embrace unpredictability.
* Think and behave in a future-friendly way.
* Help others do the same.

 It's about adopting a user-centered approach, and keeping a sharp focus on meaningful content and services.


### Progressive Enhancement

Progressive enhancement is an approach to web development that aims to deliver the best possible experience to the widest possible audience, by putting the user first. It splits web pages clearly into three bits:

* HTML for structured content
* CSS for presentation
* JavaScript for 

## Checklist

With these principles in mind, here's a checklist of things for you to apply to your own sites.

### HTML

* Use the `picture` element and `srcset` to provide the image most suitable for the user's device. You can use [Picturefill](http://scottjehl.github.io/picturefill/) to enable support for `picture` in browsers that don't support it yet.
* Every image should have `alt` text.
* Optimise your images.
* Use SVGs instead of JPGs, PNGs, and GIFs where possible.
* Use HTML5 input types like `search`, `email`, and `date`.
* Use HTML5 elements like `section`, `article`, `header`, `footer`, and `nav`.
* Use WAI-ARIA landmarks roles like `banner`, `contentinfo`, navigation, and `complementary`.
* Make sure your site is accessible. Use tools like [Tenon](http://tenon.io/) and [pa11y](http://pa11y.org/) to check.
* Be careful about your web font usage. Don't use too many, and make sure you supply a suitable fallback.
* Validate your HTML.

### CSS

* Don't use inline CSS.
* Use CSS instead of images where possible.
* Provide fallbacks for CSS features: `px` for `rem` units; `rgb` for `rgba`, suitable `background-color` for `background` images, `png` for `svg` images.
* Look at refactoring your CSS. If you have long selectors, use IDs, or over-qualify them, try refactoring using a style guide like [SMACSS](https://smacss.com/).
* Validate your CSS.
* Lint your CSS.

### Responsive Web Design

* Use a fluid grid: use `%`s instead of `px`.
* Make your images responsive, using `max-width: 100%; height: auto;`
  * Use the `picture` element and / or `srcset`.
  * Optimise your images (using a tool like [Kraken](https://kraken.io/))
* Use Media Queries to adjust elements of your site over varying screens sizes.
  * Use `min-width` rather than `max-width`.
  * Use `em` for breakpoints rather than `px`.
* Approach your site [Mobile First](http://www.lukew.com/resources/mobile_first.asp). Start with a small screen size and work your way up from there.
* Try and avoid using burgers.

### JavaScript

* Don't use inline JS.
* Place `script` elements at the bottom of the page, or load them asynchronously.
* Use feature detection (possible using a library like [Modernizr](http://modernizr.com/)) rather than device detection.
* Consider carefully if a feature is worth polyfilling. Would it be better to apply a technique like [cutting the mustard](http://responsivenews.co.uk/post/18948466399/cutting-the-mustard), and serve a simpler, faster, experience instead?
* Consider carefully if it's worth adding a jQuery plugin for a feature, rather than writing a smaller amount of code yourself.

### Performance

* Reduce sizes of CSS files by minifying them
* Reduce sizes of JS files by minifying them
* Minimise the number of HTTP requests by combining CSS files
* Minimise the number of HTTP requests by combining JS files