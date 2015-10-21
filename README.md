Optimizations made to main.js
=============================

1. Replaced jqueryselector with getelementbyid
2. Replaced jqueryselecectall with getelementbyclassname
3. Created pizzaContainer variable so I could move document.getElementByClassName("randomPizzaContainer") outside of the for loop on
   line 457.
4. Moved var dx and var newwidth out of the same for loop.
5. Changed i<100 to i<24 in the for loop on line 475 since less pizzas doesn't really change the way the original page looks.
6. Moved pizzasDiv outside the for loop on line 475 so that document.getElementById("randomPizzas") doesn't have to run multiple times.
7. Created var scroll and put it outside the for loop starting on line 509.
8. Changed i<200 to i<40 since there are only a max of 5 rows of 8 pizzas(40 pizzas) on the page at a time.
9. Changed items.length to 40 in the for loop on line 510 since items.length is constant.
10. Declared movingPizzas variable outside of the for loop on line 535.
11. Moved elem height and width from the for loop on line 533 to style.css mover class so that height and width aren't assigned 35 times.
12. Added transform: translateZ(0), transform: translate3d(0,0,0), and backface-visibility: hidden to mover class in style.css.