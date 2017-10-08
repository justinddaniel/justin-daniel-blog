---
layout: post
title:      "My first programming project"
date:       2017-10-08 20:01:27 +0000
permalink:  my_first_programming_project
---


I just completed my first programming project. I kept it relatively simple and it is mostly a proof of concept type application. I made a gem called "Adopt with Love" that scrapes from the Southwest Michigan Human Society website and, in a command line interface, offers users a list of cats or dogs available for adoption and returns the pet profile weblink of their choice. It is less than a hundred lines of code in total but is fully functioning. I also learned a lot and enjoyed making it!

My coding thus far has been specifically task-driven. For this project I had to choose my own task (within certain guidelines) and figure out my own path for achieving the functionality I wanted. I found that for its setup standing on the shoulders of giants was most useful. When we use tools developed by others rather than reinventing the wheel we are to use the phrase "standing on the shoulders of giants." I suppose programmers do this everytime they write code in some fashion or another. Without the work of countless mathematicians, the inventor of object oriented programming, etc. the work would have taken far longer. I stood on the shoulders of giants by relying on the bundler gem to give me a basic file structure to begin. 

I could then modify my file structure to my liking and begin writing the actual code. I knew I needed a CLI, a scraper class, and a controller for my CLI. That seemed the best practice based on what I learned from the lecture series by dean Avi and by the lab exercises I completed. 

As I wrote the code I overcame a number of different hurdles and learned much on the way. Why was my nokogiri scraper gem not working at first? Turns out I needed to put my required gem in the setup file that the bundler provided. Why wasn't the scraper communicating with the controler? Because I needed to make the controller an instance in the scraper class as well so they could communicate. Why was the output in the CLI not what I wanted? Because I needed to get it to print out the elements of the array line by line with the puts method rather than just return the array. 

This pattern continued for several hours. My favorite puzzle was when my .input.to_i method was unexpectedly not crashing when I fed it word strings. It turns out that it was converting even a letter input, such as "g", to the integer zero. Then when I subtracted one from the number to get the index of an array it was returning -1, and thus array[-1] would return the last element of the array! I never saw that coming. 

Writing the code for the project was a lot of fun and the puzzle-solving aspect is the essence of why I love programming so much. 




