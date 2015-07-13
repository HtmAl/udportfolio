#Project 4 - Website Performance

#Getting Started
Go to this link: (http://htmal.github.io/udportfolio/)

##Testing the default page with PageSpeed
1. Open a new tab and go to Google's PageSpeed Insights page: (https://developers.google.com/speed/pagespeed/insights/)
2. Copy the URL for my test site (see getting started) and paste it in Google's PageSpeed Insights' page to analyze it.
3. Make sure the score is above 90% for both Mobile and Desktop.

##Testing the frame rate in the pizza.html page
1. Go to this page: (http://htmal.github.io/udportfolio/views/pizza.html)
2. Open up DevTools in Google Chrome browser.

###Testing the frame rate when scrolling the page
1. Go to the "Timeline" tab in DevTools and start recording a session.
2. Scroll the page for 3 seconds
3. Stop recording the timeline and inspect the frame rate.
4. Make sure the frame rate is below 60FPS

###Testing the frame rate when selecting a different pizza size
1. Go to the "Timeline" tab in DevTools and start recording a session.
2. Move the slider near the top of the page to change the pizza size a few times.
3. Stop recording the timeline and inspect the frame rate.
4. Make sure the frame rate is below 60FPS

##Outline of performance improvements in main.js, for the pizza.html page
1. changePizzaSizes() function: Moved out of the loop some repeated code and simplified the width calculation.
2. updatePositions() function: Removed all FSL code from the for loop, simplified the math calculation needed to set the left coordinate of the pizza image.
3. DOMContentLoaded() event: Calculated the number visible of pizzas that could be shown on the screen and shrunk the original loop greatly.

See actual code for more detailed comments on this topic, thanks.
