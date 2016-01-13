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

The main.js file was improved upon and then minified. The total number of pizzas on the page was reduced from 200 to 24 and loops were optimized such that only the needed variables and functions were being declared and calculated--significantly improving performance. In addition query selectors were substituted with the more efficient getElementById. Painting on the pizza page was improved upon using the hardware accelerated CSS "will-change:transform.""  Basic changes were also made to pizza.html (moving and minifing styles and scripts) to improve performance. Cam did NOT make the layout of pizza.html responsive including NOT including a viewport meta tag. What a shame.

* Time to generate pizzas on load: 17.685000000000002ms
* Time to resize pizzas: 0.9099999999962165ms
* Average time to generate last 10 frames: ~0.2309999999975844ms
* PageSpeed Insights Desktop: 98/100

Shout out to Cameron Pittman. That guy has taught me an unreal amount.
