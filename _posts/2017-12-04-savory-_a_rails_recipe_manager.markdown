---
layout: post
title:      "Savory- A Rails Recipe Manager"
date:       2017-12-04 08:59:27 -0500
permalink:  savory-_a_rails_recipe_manager
---


I've grown to really love and appreciate the portfolio project section of the learn curriclum, for the sole fact that they will almost always reveal to you just how much you actually dont understand and challenge you to learn it quickly by building. 

As always with any portfolio project, the hardest part of starting was coming up with an idea. This program has made me realize I am not an idea person, however I am an idea executer and I'm ok with that. Originally when I started my Rails project the teaching expat community here in Korea had been shook, the lesson plan sharing website everyone had used freely for 11 years, locked everyone out without warning and charged a fee to gain access to user- made content. It was devestating and absolutely nothing anyone could do about it. I really wanted to do something about it, I wanted to use my rails portfolio project as an opportuntity to build something really useful for the teachers here in Korea. I started the project, but trying to make it fit the requirements and be what teachers needed it to be proved too difficult, so I decided to shelve the idea for the time being, and focus on making something that could easily fit the requirements. In the end I decided on a recipe manage because it was one of the suggested projects and I recently started cooking more.

Nested forms were extremely difficult for me to get working. I didnt know how much I didnt understand nested forms until I had to incorporate the into my application. One of the hardest things was getting my custom attribute writer to work correctly. I chose to write my Ingredient model for the custom attribute, but for the life of me in the beginning I could not get the ingredient name attribute to save to the database. I has no idea what I was doing wrong, through some googling I realized in my recipe_ingredients table, I had "ingredients_id" instead of "ingredient_id", so that helped to solved that, however I still ouldnt get my custom attribute to work, I could only get my app running correctly initally through accepts_nested_attributes_for, and rearranging something in my whitelist params in my recipe controller. Eventually through some research and a stroke of luck, I got my ingredients custom attribute writer working. And thus was able to fulfill the requirement of having a nested form write to one associated model using a custom attribute writer.

The second most confusing thing for was trying to figure out what a scope was, but after checking the rails documentation and seeing a few examples, I was able to come up with a scope method pretty easy. 

This project definitely was a learning experience. A few new things that I learned :

1.Push to Heroku EARLY AND OFTEN. Once I got my basic crud fuctions working, I put my project on Heroku and thank God that I did, because had I waited until the last minute the number of issues I would have encounter would have completely overwhelmed me.
2.Speaking of Heroku, while working on the project I had the pleasure of learning that Heroku only stores images upload through paperclip temporarily, so once you logout the images are gone, to remedy that I had to learn how to use AWS-S3 and S3 bucket, and man was that a steep learning curve trying to get that to work, especially while outside of the United States, but I did and will definitely be writing a blog on that later.
3. Getting Facebook Omni-Auth working both in development and production also posed it's challenges, but I was able to achieve that as well, and defintiely plan to write a blog post on that as well.
4. Another thing that was a learning experience, was getting my video back-ground to work both locally and on Heroku, that took a lot of research to get up and running, but I am happy with the knowledge I've gained from trying something outside of my comfort zone. 

My project is pretty much complete as far as the requirements go, but as I work on it over time, there are still a few things, that I would like to improve, like the design and customizing devise so that users who sign in through facebook can make edits to their account and change their currently devised generated password. But for now on to Javascript!
