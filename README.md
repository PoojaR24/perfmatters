## Website Performance Optimization portfolio project

Open index.html in a browser
My project can viewed at https://poojar24.github.io/perfmatters/

NOTES BY POOJA.R
================

SHORTENING THE CRITICAL RENDERING PATH
- added async attribute to the google analytics script
- inlined the perfmatters.js script
- minified and inlined the styles from style.css and print.css files
- moved the google font link to below the footer
- optimized and resized the pizzeria.jpg for the index.html

PIZZERIA
- changed the items[i].style.left to transform and transalte to improve FPS
- moved the items variable down below the anonymous function that generates the sliding pizzas
- also made the items variable available globally by adding window.items = document.querySelectorAll('.mover');
- implemented requestAnimationFrame as described in http://www.html5rocks.com/en/tutorials/speed/animations/ implementation starts at line 500 of main.js
- removed the dx variable declaration from the changePizzaSizes function for loop
- removed document.querySelector("#movingPizzas1") from the event listener anonymous function and into its own variable (line 548)
- Inlined the style.css for pizza.html to unblock critical rendering path
- added <meta charset="utf-8"> and <meta> viewport tags to pizza.html
