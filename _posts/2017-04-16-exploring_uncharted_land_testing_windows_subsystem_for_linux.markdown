---
layout: post
title:  "EXPLORING UNCHARTED LAND: TESTING WINDOWS SUBSYSTEM FOR LINUX"
date:   2017-04-16 10:14:23 +0000
---


I was pretty bummed out when I learned that Ruby and Windows doesn't play well together and that I would more than likely need to either dual boot or switch my OS entirely. I looked into dual booting, but a lot of the information I was reading made it seem a bit complicated and sort of risky. I was very afraid of messing up my windows installation somehow and breaking my computer. It also seemed like it would be a pain to reboot every time I wanted to switch between the 2 operating systems.

So I looked for more options and ultimately decided to give windows subsystem for linux a try. This gives me a fully operational Linux Bash Shell running natively on my Windows laptop. It enables me to: 1. Have full access to both my Linux and  Windows file-systems from both Bash on Windows and File Explorer. 2. Not have to reboot to switch between windows and Linux. 3.Not run the risk of messing up my windows installation, because this is an official microsoft product. All in all windows subsystem sounds pretty dreamy right?!?!

Weeeellll.....not exactly! Window's Subsystem is still in beta, which means that everything doesn't always one hundred precent work correctly and there are still a few bugs that need to be fixed and not a lot of documentation out there to help you trouble shoot if you run into a unique issue. I am not an experience linux user so I can't say how far off from the real thing WSL is, but I feel like for what I am trying to accomplish with Flatiron's curriculm, WSL should be able to get it done without too many problems. 

So to setup the ruby enviornment I'll be needing to complete the learn curriculm, I followed the [Gorails.com tutorial](https://gorails.com/setup/windows/10) on setting up ruby and ruby on rails on WSL. For the most part it was an easy process, but sort of slow. It took about 4 hours to get everything installed. I installed a ruby version manager called rbenv as recommend, but there was another choice called RVM. Waiting for rbenv to install took an hour and 10 minutes, after that I had to install ruby-build and then finally Ruby, which also took a while to install. From there I installed Nodejs which is suppose to help by minifying my javascript and providing a faster production environment. Then next came Rails,which was easy to install. Afterward I was ready to launch my first test rails app to see if everything was working. Unfortunately everything wasn't working, I couldnt get my localhost to connect to my rails server. I had to do a bit of searching on stack overflow and github to fix my problem, but in the end I was able to find a solution. 

I am hoping that even though WSL is pretty much uncharted land and every day new bugs are found and fixed, that it is a blessing for me and I wont have to dual boot or switch out my operating system. So far so good, there are a few things I will have to get use to, but I'm up for the challenge. Here's hoping I can be one of the pioneers that helps WSL catch on and improve. 
