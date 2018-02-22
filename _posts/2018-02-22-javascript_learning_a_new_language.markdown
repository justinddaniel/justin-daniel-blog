---
layout: post
title:      "Javascript: learning a new language"
date:       2018-02-22 23:05:52 +0000
permalink:  javascript_learning_a_new_language
---


Having completed my rails with javascript project I can reflect on the pecularities of the language and my experience learning it. The first thing I noticed about it is that it is not a pure object oriented language like Ruby is; creating classes of objects seems much clunkier. It also feels as though chaining functions/methods together is more cumbersome than Ruby, but perhaps this is more a reflection of the greater experience I have with Ruby. 

I understand the importance and the great capabilities of javascript though. Dynamically changing the DOM without a page refresh is quite amazing; I can remember my early teenage years and how whenever I wanted to get more emails or see more information on a webpage I needed to wait for a full reload/refresh or be redirected to yet another page. Something changed, as I recall, in the late 90's and early 00's and that something was Javascript. 

The best means of consolodating my learning seems to again be the projects, and side-coding on codewars to solve some unique problems. One of the biggest roadblocks I ran into in this latest project is the $(this) selector. For several hours I kept returning the window as 'this' in spite of my best efforts. I had to do some serious reading and understand that the function called within my eventListener function was called in the global scope and that this was changing the 'this' selector. I found a way around this problem by setting a global variable dynamically within the function scope and using that later on with the data that I needed.

Scope is a weird thing in Javascript. I certainly understand the use of having a local scope be able to pull from the global scope and not vice-versa; I do not want my local variables in the global scope. But why the differences between "let", "const", and "var"? Hoisting seems inconsistent. I read in another source that using arrow functions () => can produce different $(this) outcomes than function () {}. Apparently this was fixed in the 2015 update, but not wanting to take a chance I stayed away from arrow functions for one of my methods, even though I like the look of the syntax better. 

I still have a lot I want to learn about Javascript but I at least feel that I can now do the basics, having knocked out the project and having a dozen or so codewar JS challenges under my belt. 
