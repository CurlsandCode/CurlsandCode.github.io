---
layout: post
title:  "Wanderlist - A Travel CRUD App"
date:   2017-07-17 11:43:35 +0000
---

![](https://scontent-hkg3-1.xx.fbcdn.net/v/t1.0-9/20108612_1829377567072709_5102245629416902957_n.jpg?oh=baa38bab74e1486396e077a9c8a1b826&oe=5A069150)

After almost two weeks of triumphs and challenges, I have finished my Sinatra CRUD app. This project was really fun to complete, but also extremely trying at times. I thought it would be easier to get started because this is my second project, but no, blank files still intimidate me, so even though I ultimately knew what I wanted to do, starting from a blank file made me hesitant to start. Eventually I was introduced to the wonderful Corneal gem that was created by a previous Flation student and began my project. 

So I the criteria for the was to create a CRUD app that tracks something important to you, so naturally I chose travel. I love traveling and I consider it a big part of who I am as a person. My CRUD app Wanderlist, a play on the word Wanderlust, lets users keep track of places they want to visit. It sounds simple enough, but I ran into a whole host of problems along the way that had me wanting to pull my hair out.

One of the main problems I had was trying to figure out the associations between models. When I first started the project I figured users would have a list and add places to that list, but as I started to work on it, it felt like I was writing a previous lab I had done, so I decided that users would have two list, one for places they've been and one for places that they want to go. Ultimately that made my associations a little more complicated and harder for me to figure out what was best. I tried:
```
user 
has_many :list
has_many :places through: :lists
list
has_many :places
belongs_to :user
places
belongs_to :list 
belongs_to :user
```
but that wasn't really working, so then I tried:
```
user 
has_many :list
has_many :places through: :lists
place
has_many :lists
has_many :users, through: lists
list
belongs_to :place
belongs_to :user
```
My app worked a little better with my assocations set up this way, but when a user created a new place on the list for Places they've been, it would automatically also be added to the places they wanted to go, which was not how the app was intended to function. So after banging my head against a wall, I sought out help. I set up office hours with Cernan and he formed me that it would be better to use a join table and a boolean to properly be able to differentiate what places should go on what list. So my finial associations looked like this:
```
user
 has_many :user_places
has_many :places, through: :user_places
place
has_many :user_places
has_many :users, through: :user_places
user_places
belongs_to :user 
 belongs_to :place `
```
Ultimately this made more sense then my previous associations, but taking out the list model and using a boolean to decided wether it was a place a user had been or wanted to go, just wasnt registering with me, I couldn't figure out how to generate two static list for every user that could be populated based on if the boolean attached to the places was true or false, so I went back to plan A, just focusing on places a user wants to go. After getting my assocaitions sorted and deciding to focus on one thing, it was pretty much smooth sailing from there, and I only encountered a few minor bugs that were easily solved.

I like how this project turned out functionally, because it does everything it's suppose to do, but I love how this project turned out aesthetically. It's not quite mobile responsive, yet, but on desktop, it really came out nice and solidified my love for front-end development more than back-end. Overall I learned a lot while bringing this project to life and I'm glad I had a chance to dig deeper into Sinatra.
