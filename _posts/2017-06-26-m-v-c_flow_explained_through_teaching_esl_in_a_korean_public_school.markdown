---
layout: post
title:  "M-V-C Flow explained through teaching ESL in a Korean public school"
date:   2017-06-26 08:28:04 -0400
---


![](https://scontent-hkg3-1.xx.fbcdn.net/v/t1.0-9/12814639_1207734799236992_7981379635864329554_n.jpg?oh=8800c415f168c337a325b82c4a19a1ed&oe=59E08F5A)


   When I first started the Sinatra section and learned about the Model-View-Controller Pattern, I immediately thought "Hey this sounds exactly like what it is like to teach English in a public school in South Korea", which is my current job by the way. 

If you've never taught English in South Korea, you might be a little confused by that comparison, so I'm going to due my best to explain how I can relate one to the other. 

This semester we recieved about 25 new teachers to our school, and like most Korean people I meet they were eager to meet me and eager to learn English, so eager in fact that they asked me to teach an after school teacher's English class. 

This  small interaction can be equated to the first step in Basic MVC flow : 1.The user interacts with our application's view(s) via the command line or a web browser. The user enters some input that asks our application to show them for example a list of all of their friends who are using the application. So basically in this first step the user(s) is/are my korean co-workers and I am the view. They are requesting  for me to prepare a teacher's english class for them to view and gain information from. 

Now, as a foreigner in Korea I don't have any power to make their request happen all on my own, for any request or service to be rendered by me it must go through my co-teacher. My co-teacher acts as a go-between, between me and the students, the other teachers, and my school principal. My co-teacher translates important information and requests from english to korean and from korean to english.

So this is basically like the second step in Basic MVC flow : 2.The controller receives this request and looks at it. The controller says, "Okay, this user wants to see a list of their friends." You can conclude the controller in this analogy is my co-teacher. Also, just like any complex application has multiple controllers, I have multiple co-teachers. 

My co-teacher also has very little power in making things happen and they must also run the request by the school's principal and the principal will check my contract and then respond with a 200 or a 404, haha, no but seriously they either tell my co-teacher yes, the request is possible or no, it's not in the contract so it can't be rendered. 

This is like the third and fourth step in Basic MVC flow: 3.The controller then asks the Friends model to go into the database and return all of the user's friends. 4.The model goes to the database, retrieves all of the requested data, and gives it to the controller. So my principal takes on the role of the model and my contract is her database.

Once my co-teacher was informed that I could teach an after school teacher's english class, I put together a few powerpoints and presented english lessons to my teacher's class. 

This is like the fifth step in Basic MVC flow: 5.The controller passes that data to a view, and the view displays it to the user. With of course my co-teacher acting as the controller, me as the view, and the teachers as the user(s).

This may seem like a strenuous process to get things done, but considering I don't speak Korean and my principal nor do all of my students or other staff members speak English, the MVC way of communicating works here.

So just a quick run down incase you still dont see the connection:

   * ** Models :** The 'logic' of a web application aka My school principal, she makes the descisons about what I can and can't do and can use my contract aka the database to pull that information from. 
* **Controllers:** The go-between for models and views aka My co-teacher, she translates request from korean to english and english to korean, making it so myself and the principal never interact directly with each other. 
* **Views:** The part of the app that the user interacts with directly aka me, I am put on display for the user(my students) to gain information from and make request to. 

 And that is how MVC flow is like teaching English in a South Korean public school.


![](https://scontent-hkg3-1.xx.fbcdn.net/v/t1.0-9/21704_1226677887342683_6628784948398340290_n.jpg?oh=4cb7f130ead90a83f5d7d243d514ebe9&oe=59D96912)
