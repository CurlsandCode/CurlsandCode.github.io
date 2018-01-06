---
layout: post
title:      "Animation on scroll - integrating AOS.js with my Rails app"
date:       2018-01-06 07:30:50 -0500
permalink:  animation_on_scroll_-_integrating_aos_js_with_my_rails_app
---


While trying to figure out how to incorporate WOW.js in my Rails application to give my scroll some pizzazz I came across AOS.js. It is super easy to ingerate into a rails, but there isnt very much information avaliable about how to do so, so I figured I'd do my part and share how I did it. 



AOS.js github:

http://github.com/michalsnik/aos

First start by adding the following to your application.js file:

![Imgur](https://i.imgur.com/fNv6XIL.png)

Then add this line, `<link href="https://cdn.rawgit.com/michalsnik/aos/2.1.1/dist/aos.css" rel="stylesheet"> `  to your application.html.erb header. like so:

![Imgur](https://i.imgur.com/ZLVdFii.png)

Then chose one of the many animations, check them out live here :http://michalsnik.github.io/aos/
Add  it to your view: 
![Imgur](https://i.imgur.com/XahL5l8.png)

Then at the bottom of your view add:
![Imgur](https://i.imgur.com/Ey3Vi93.png)

And that's how you add cool scrolling animations to your rails app,using AOS.js! 

For more info on AOS.js check out these articles:
https://css-tricks.com/aos-css-driven-scroll-animation-library/
https://www.sitepoint.com/cool-scroll-animations-made-easy-aos-library/
