title: Cascading Style Sheets
category: page
slug: cascading-style-sheets
sortorder: 0417
toc: False
sidebartitle: Cascading Style Sheets (CSS)
meta: Learn how to use Cascading Style Sheets (CSS) to create your web application's user interface design on Full Stack Python.


# Cascading Style Sheets (CSS)
Cascading Style Sheet (CSS) files contain rules for how to display and 
lay out the HTML content when it is rendered by a web browser.

<img src="/img/logos/css.jpg" width="100%" alt="CSS3 logo." class="shot">


## Why is CSS necessary?
CSS separates the content contained in HTML files from how the content 
should be displayed. It is important to separate the content from the rules
for how it should be rendered primarily because it is easier to reuse those
rules across many pages. CSS files are also much easier to maintain on large
projects than styles embedded within the HTML files.


## How is CSS retrieved from a web server?
The HTML file sent by the web server contains a reference to the CSS file(s)
needed to render the content. The web browser requests the CSS file after the
HTML file as shown below in a screenshot captured of the Chrome Web Developer 
Tools network traffic.

<img src="/img/visuals/css-chrome-dev-tools.jpg" width="100%" alt="Google Chrome Web Developer Tools shows how CSS is separate from the HTML content." class="shot rnd outl">

That request for the fsp.css file is made because the HTML file for Full 
Stack Python contains a reference to ``theme/css/fsp.css`` which is shown
in the view source screenshot below.

<img src="/img/visuals/fsp-css-source.jpg" width="100%" alt="View source screenshot for the fsp.css file in index.html." class="shot rnd outl" />


## CSS preprocessors
A CSS preprocessor compiles a processed language into plain CSS code. CSS 
preprocessing languages add syntax such as variables, mixins and functions
to reduce code duplication. The additional syntax also makes it possible for
designers to use these basic programming constructs to write maintainable
front end code.

* [Sass](http://sass-lang.com/) is currently the favored preprocessor in
  the design community. Sass is considered the most powerful CSS preprocessor
  in terms of advanced language features.

* [LESS](http://lesscss.org/) is right up there with Sass and has an ace up
  its sleeve in that the [Bootstrap Framework](http://getbootstrap.com/) is
  written in LESS which brings up its popularity.

* [Stylus](http://learnboost.github.io/stylus/) is often cited as the third
  most popular CSS preprocessing language.


### CSS preprocessor resources
* The Advanced Guide to HTML and CSS book has a well-written chapter on 
  [preprocessors](http://learn.shayhowe.com/advanced-html-css/preprocessors).

* [Sass vs LESS](http://css-tricks.com/sass-vs-less/) provides a short answer
  on which framework to use then a longer more detailed response for those
  interested in understanding the details.

* [How to choose the right CSS preprocessor](http://blog.teamtreehouse.com/how-to-choose-the-right-css-preprocessor)
  has a comparison of Sass, LESS and Stylus.

* [Musings on CSS preprocessors](http://css-tricks.com/musings-on-preprocessing/)
  contains helpful advice ranging from how to work with preprocessors in a
  team environment to what apps you can use to aid your workflow.


## CSS libraries and frameworks
CSS frameworks provide structure and a boilerplate base for building a
web application's design.

* [Bootstrap](http://getbootstrap.com/)

* [Foundation](http://foundation.zurb.com/)

* [Gumby](http://gumbyframework.com/)

* [Compass](http://compass-style.org/)

* [Profound Grid](http://www.profoundgrid.com/)

* [Skeleton](http://www.getskeleton.com/)

* [HTML5 Boilerplate](http://html5boilerplate.com/)


## CSS resources
* [Frontend Development Bookmarks](https://github.com/dypsilon/frontend-dev-bookmarks)
  is one of the largest collections of valuable resources for frontend
  learning both in CSS as well as JavaScript.

* [CSS Reference](https://cssreference.io/) provides much-needed visual 
  examples for every CSS property to show you what they are actually going 
  to look like on your pagee when you use them.

* [CSS coding techniques](https://hacks.mozilla.org/2016/05/css-coding-techniques/)
  provides advice on how to write simpler, easier-to-maintain CSS code
  to reduce your need to rely on CSS preprocessors and build pipelines.

* [CSS refresher notes](https://github.com/vasanthk/css-refresher-notes) is
  incredibly helpful if you've learned CSS in bits and pieces along the way
  and you now want to fill in the gaps in your knowledge.

* [Mozilla Developer Network's CSS page](https://developer.mozilla.org/en-US/docs/Web/CSS)
  contains an extensive set of resources, tutorials and demos for learning
  CSS.

* [CSS Positioning 101](http://alistapart.com/article/css-positioning-101)
  is a detailed guide for learning how to do element positioning correctly
  with CSS.

* [Learn CSS layout](http://learnlayout.com/toc.html) is a simple guide that
  breaks CSS layout topics into chapters so you can learn each part one
  at a time.

* [Google's Web Fundamentals class](https://developers.google.com/web/fundamentals/)
  shows how to create responsive designs and performant websites.

* [Tailoring CSS for performance](http://programming.oreilly.com/2014/04/tailoring-css-for-performance.html)
  is an interesting read since many developers do not consider the 
  implications of CSS complexity in browser rendering time.

* [Can I Use...](http://caniuse.com/) is a compatibility table that shows
  which versions of browsers implement specific CSS features.

* The [Web Design Museum](https://www.webdesignmuseum.org/) is an amazing
  look back at how web design has evolved over the past 25+ years. Some of 
  the designs can still be seen in their current site's presentation such
  as the top navigation of Apple's 2001 site.


## CSS learning checklist
1. Create a simple HTML file with basic elements in it. Use the
   ``python -m SimpleHTTPServer`` command to serve it up. Create a 
   ``<style></style>`` element within the ``<head>`` section in the HTML
   markup. Play with CSS within that style element to change the look and 
   feel of the page.

1. Check out front end frameworks such as Bootstrap and Foundation and integrate
   one of those into the HTML page.

1. Work through the framework's grid system, styling options and customization
   so you get comfortable with how to use the framework.

1. Apply the framework to your web application and tweak the design until you
   have something that looks much better than generic HTML.

