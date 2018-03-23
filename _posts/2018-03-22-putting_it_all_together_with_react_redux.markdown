---
layout: post
title:      "Putting it all together with React/Redux"
date:       2018-03-23 02:20:21 +0000
permalink:  putting_it_all_together_with_react_redux
---


Phew! The past four days have been pretty intense! It has been enjoyable though; I like challenging my brain and pushing it to its limits. I have made an App called Deflator that helps with tracking diet and exercise and can therefore be useful for trying to lose weight. Hence its funny name of 'deflator' (hard to believe it was not already taken on github). I had to put a lot together for this. 

I have never made a separate API and client-side server before. Thank goodness for the genuises who came up with Rails new and react-create-app. With some online guides I got past that fairly quickly. Getting them to play nicely with each other took some time though. At first it appeared that foreman would do the job. But yesterday my fetch calls started failing and during office hours I figured out with an instructor that I needed the cors gem. Once that was installed and wired properly then my fetch calls could go through. 

There were some distinct phases in my project coding. I first coded in plain React following some simple patterns. Once I wanted Redux added on though I needed to do a lot of refactoring. It took time, but my app was a lot faster once that was done!

Finally I had to add the Router. At first this seemed just like some kind of alien language to me but after watching a couple of videos, reading a few articles, and then testing it out on my own, I finally got it. I was amazed at how quickly pieces of the DOM could be switched out with simple clicks of buttons and links. I definitely see the advantages of this power combo of React, Redux, Redux middleware and connect, and Redux Router. 

There is plenty more I want to add to my app. Thus far users can add themselves to the database and enter in their goals, calorie allotments, and some other traits. I eventually want to make it so they can add in their own journal and track their foods, exercises, and net calories daily. 


