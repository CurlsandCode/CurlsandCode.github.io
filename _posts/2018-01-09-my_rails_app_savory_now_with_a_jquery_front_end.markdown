---
layout: post
title:      "My Rails app, Savory, now with a jQuery Front End"
date:       2018-01-09 10:02:07 +0000
permalink:  my_rails_app_savory_now_with_a_jquery_front_end
---


I really hoped that this project would be easier  to get through than the last 3, but sadly I had just as many challenges as with the previous projects. It was my faught though I didn't know what I was getting myself into when I got all image happy and wanted pictures all throughout my app. Normally before every project I like to browse github and checkout other flatiron students projects(the ones with links to heroku), I was always surprised with the lack of images used, but I figured that maybe the other students didnt want the headache of configuring paperclip, heroku, and the aws-sdk gem, I never thought to think how difficult using images can make things, especially when you are mixing languages. One of my biggest hiderances with this project was rendering pages using javascript and getting them to look the way I made them in Ruby. For example, when I started this project, I had a clear plan for how I would meet the requirements, I would add a read more button on the recipe index page, and I would ask a next button on the show page, and to meet the last requirement I would create a comment resource and render that on the recipe show page without a refresh. The more button was super easy to add, because I already had practice from a previous lab, but the next button was a no-go, I tried so many ways but I couldnt get it working, so I went to plan B, I would meet the requirement by rendering a recipe showpage without a refresh from the recipe index page. I actually got that working, but heres the thing my beloved images would not coporate, I couldn't get my template literals to behave how I wanted them to. When I created the recipe show page in rails it looked like this :

![Imgur](https://i.imgur.com/vVi8jm8.png)

However when I tried to recreate that page with template literals and have it rendered without a page resource the best I got was this:

![Imgur](https://i.imgur.com/fNIskbf.png)

It was close, and maybe my learn instructor would have taken pity on me and counted it as meeting the requirement, since my javascript code did work, just the rendered results aesthetic were displeasing, but no, I decided to once again scrap that code, and try a different way to meet the requirement. I ultimately decided to create a user profile page, with very limited design and image use, so that I could render it easily with template literals. 

One other thing that really stumped me and had me struggling for days was whenever I made a comment on a recipe the username would append  to the page as undefine, and then I would refresh the page and the username would appear. I deleted, wrote, and rewrote my comments code many times and many different ways, only to keep getting the same response. And then I read something on a stack overflow question and it made me think of what the problem could possibly be. So in my user serializer I wrote a method that changed the user attriute to return a user's username. I forgot about that, so when I built my comment prototype, I was calling this.user.username, which in turn turned out to really be calling username.username, which is why it was apprending as undefined.  Overall this project was hard, javascript is not my strong suit, and I definitely need to practice using it more and put more energy into understanding it. Next up is React and I'm sure that'll be a beast, but I'm looking forward to working with it.
