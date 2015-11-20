### Website Optimization Project
This is a project from [Udacity](https://www.udacity.com)'s [Front-End Web Developer Nanodegree](https://www.udacity.com/course/front-end-web-developer-nanodegree--nd001).

### How to view the project
Click [here](http://dbhkhk.github.io/frontend-nanodegree-mobile-portfolio/).
This site is optimized to achieve a score over 90/100 for the [analysis from PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fdbhkhk.github.io%2Ffrontend-nanodegree-mobile-portfolio%2F).

In the portfolio page, you can find the link to the [pizza page](http://dbhkhk.github.io/frontend-nanodegree-mobile-portfolio/views/pizza.html),
which is optimized to achieve 60 FPS when scrolling the page and less than 5 ms when resizing pizzas on the page.

### Optimizations
#### in index.html
1. inline style.css and print.css
2. add "async" to script tags
3. comment out google font
4. resize images to reduce bytes

#### in views/js/main.js
1. move code involving layout out of for loops to avoid forced synchronous layouts (FSL)
2. add randomPizzaContainers to avoid repeating work
3. redesign the algorithm for changing pizza sizes to avoid FSL and save unnessesary work
4. add "use strict"
5. replace querySelectorAll by getElementsByClassName
6. replace querySelector by getElementById
7. save *.length in for loop conditions in var len
8. move declaration of pizzasDiv, elem, and movingPizzas1 outside the loop
