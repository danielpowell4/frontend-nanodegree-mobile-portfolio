Website Performance Optimization portfolio project
==========================================================

This project for Udacity's FEND nanodegree, is all about optimizing the critical rendering path and making these page render as quickly as possible. It is the capstone for this course: [Critical Rendering Path course](https://www.udacity.com/course/ud884).

View the Landing Page [here](http://danielpowell4.github.io/frontend-nanodegree-mobile-portfolio/)
View the Jank-free Pizzeria Site [here](http://danielpowell4.github.io/frontend-nanodegree-mobile-portfolio/views/pizza.html)

Part 1: Optimize PageSpeed Insights score for index.html
===============================================================

When last checked, PageSpeeds gave the Mobile and Desktop scores at 96 & 97 respectively. This was done in large part by hand. Tools like grunt were not applied.

* Stylesheets were minified using [cssminifier.com](https://cssminifier.com/) and placed in the header as they wouldn't be used elsewhere
* Scripts were minified using [jscompress.com/](http://jscompress.com/) and moved to the bottom of the body as appropriate
* Images were compressed losslessly using Adobe Photoshop's "Save For Web Feature" and some magick

Part 2: Optimize Frames per Second in pizza.html
===============================================================

The main.js file was improved upon and then minified. Specifically loops were optimized such that only the needed variables and functions were being declared and calculated--significantly improving performance. Basic changes were also made to pizza.html (moving and minifing styles and scripts) to improve performance. Cam did NOT make the layout of pizza.html responsive including NOT including a viewport meta tag. What a shame.

* Time to generate pizzas on load: 20.725000000000023ms
* Time to generate pizzas on load: 20.725000000000023ms
* Average time to generate last 10 frames: ~1.6610000000007858ms
* PageSpeed Insights Desktop: 98/100

Shout out to Cameron Pittman. That guy has taught me an unreal amount.
