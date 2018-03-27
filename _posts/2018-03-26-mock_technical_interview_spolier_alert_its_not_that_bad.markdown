---
layout: post
title:      "Mock Technical Interview: *SPOLIER ALERT* (It's not that bad!)"
date:       2018-03-27 01:49:08 +0000
permalink:  mock_technical_interview_spolier_alert_its_not_that_bad
---


I graduated last week and I must say the feeling was incredible. However, my work isn't done yet, the next step in my mission to change careers is to actually get a job, and to get a job, I like every developer before me must learn how to ace the technical interview. 

A nice perk of being in Flatiron's Online immersive is the chance to do a mock interview on the interview site Skilled, for free. I graduated on Wednesday and scheduled my mock interview for the following Saturday. I was of course nervous, I knew that the interview would more than likely consist of a few javascript trivia questions, basic cs trivia, and a few whiteboard problems. Even though my career coach told me not to study,because the mock interivew is suppose to be a snapshot of where you are, I still attempted to try to study what I thought might be asked. 

When my interview started my heart was racing, I was trying to appear calm, but I could feel my palms getting sweaty and my mouth getting dry. My interviewe Craig was warm and friendly, he introduced himself and gave me his background story. He told me we would just be focusing on vanilla javascript for this mock interview. 

He explained how the code editor worked and jumped right into whiteboarding. I was a little shocked because I thought he would start me off with some trivia, but nope, the first task he gave me was to reverse a string. My heart start to eat at a normal pace, I definitely knew how to reverse a string. I had learned that way early on in my Free Code Camp Days.

I promptly wrote: `function reverseStr(str) { return str.split(" ").reverse( ).join(" "); }`

Then he ask me to reverse the string without using the reverse method, which was also within my comfort zone. So I wrote this: `function reverseStr(str) { let reversed=" "; for(let i= str.length-1; i >=0; i--){ reversed+= str[i] } return reversed; }`

Then we left the safety and warmth of my comfort zone, when he ask me to *Write a function to reverse each word in a string keeping each word in it's original order, example : "The cat is fat" becomes "ehT tac si taf*

Sounds easy enough, I knew I needed an array, but I still couldnt figure out what difference an array would make in helping me to keep the words in order, because with a plain reverse function I was getting * ' taf si tac ehT'.  I was completely stuck and not picking up on hints. Eventually the interviewer showed me how to solve it by piggybacking off my original reverseStr function:
`function reverseSentence(str) { let arr = str.split(' '); for(let i= 0; i < str.length; i++){ arr[i] = reverseStr(arr[i]); } return arr.join(' '); }`

Then we moved to the next question which went even further out of my comfort zone: *Write a function to break a string up into 5 character long segments and return them as elements in an array, basically like setting a 140 character tweet limit*.
I felt like the Mister Crab meme!


![](http://i0.kym-cdn.com/entries/icons/facebook/000/020/001/krabs.jpg)

 I knew I would need an array, a for loop, and an if statement, but I wasn't sure how I could compare the character count as it was input into the array and decide if it has reach its limit and to start over with a new string. Once again I was stuck. So eventually the interviewer ended up showing me how to solve the problem: `function tweetCount(str){
let arr=[]; let temp=' '; for(let i= 0; i < str.length; i++ ){ temp+= str[i]; if (temp >= 10){
temp = ' '; } if(temp > 0) {
arr.push(temp) } return arr; }`

The last question he asked was given this function `(function(){ var a= b=3; })();` which is defined a, b, or both? I was really happy to get this question because after two failed problem solving attempts I was ask something within my comfort zone.  Thanks to Flatiron's wonder emphasis on Hoisting and Scope during the Jquery Assessment, I knew hoisting really well, so I was able to reason pretty quickly that due to the rules of hoisting and scope a would return undefined and b would return 3! My interview was at least impressed with my hoisting knowledge, he told me out of the last 20 people he ask that question to, I am the only one that gave the correct answer! So I was pretty happy with that! 

Overall I did pretty bad in my first Mock interview, but I definitely learned a lot. My interiewer was a really great guy, never once did he make me feel like me not knowing how to solve the problem equated to me being stupid or not knowing how to code at all. He was patience and kind and gave me a lot of great advice and encouragement. I have a lot to work on, but at least I know exactly where to start. I will tame the beast that is algorithms. I will improve my problem solving  and live coding skills. And the next time I am faced with either of those questions I failed in another interview, I will knock them out of the park. 
