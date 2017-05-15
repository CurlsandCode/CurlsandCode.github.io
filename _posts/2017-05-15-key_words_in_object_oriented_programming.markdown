---
layout: post
title:  Key words in Object Oriented Programming
date:   2017-05-15 05:40:37 +0000
---

![](https://cdn-images-1.medium.com/max/800/1*cBFSQ9Ytv_D0jwGtpuL5WA.png)

As I am nearing the end of object oriented programming, I can safely say that I am NOT A FAN! When I first started to feel like object oriented programming sucked, I wondered if I was in the minority, if something was wrong with me. Why was I not able to bask in all the benefits that everyone told me OOP offered? Luckily google is always available to help you find your tribe and that's just what I did. I found many other programmers, who also felt  loathing when it comes to OOP, even some very prominant computer programmers have expressed their distaste for OOP. Two of my favorite quotes: 

> "Object-oriented programming is an exceptionally bad idea which could only have originated in California."-Edsger W. Dijkstra


> "The problem with object-oriented languages is they’ve got all this implicit environment that they carry around with them. You wanted a banana but what you got was a gorilla holding the banana and the entire jungle."- Joe Armstrong

Even with my preference of procedural programming, I still had to push through and try to gain a working knowledge of Object Oriented Progamming and complete this section of learn. One thing I noticed with OOP, a lot of the directions reminded me of word problems in math. 

For example Here is the word problem you see on the test and the number sentence you need to formulate  in order to solve it :
> 
> Word problem: “Sue has two pencils. She spends one hour at the store and buys three more pencils. How many pencils does Sue have in all?”
> 
> Number sentence: “2 + 3 = ____.”

Word problems in math can be solved by recognizing the keywords that indicate what mathematical operations you need to solve the problem. Here is a table of examples: 

![](http://media-cache-ec0.pinimg.com/736x/56/39/ed/5639edb48990f9c05d7fc1450c85b47a.jpg)

The hardest thing about OOP for me was remembering the major keywords and what action they indicated to preform. SO here is a sort of cheat sheet I came up with to help me remember:

1.**Class**- 
> ```
 class Myclass
 #block of code            
 end
```


2.**Instantiate**- `class.new `

3.**#method**
```
def name
#block of code
end
```

4.**Instance variable**- `@variable_name`

5.**Setter**- 
`def name=(your_name)
@this_guys_name = your_name
end`

6.**Getter**-
```
def name
@this_guys_name
end
```

7.**attr_reader**- `:name`, creates a getter method

8.**attr_writer**- `:name` , creates a setter method

9.**attr_accessor**- `:name` , creates a setter and getter method

10.**Initialize**-
```
def initialize(arg)
@arg =arg
end
```

11.**Class Constant** - `NAME`

12.**Class Variable** -`@@variable_name`

13.**Class Method**-
 `def self.class_method_name
 #block of code
 end`
 
  These are just a few keywords that have appeared in learn labs, and at first it was confusing to remember what they meant, but now I have a pretty good grasp on these words and what they indicate I should be doing in my program. I may not like object oriented programming, but I do understand it. 
