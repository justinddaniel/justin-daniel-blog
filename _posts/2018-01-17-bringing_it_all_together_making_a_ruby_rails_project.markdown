---
layout: post
title:      "Bringing it all together: making a Ruby Rails project"
date:       2018-01-17 17:08:40 +0000
permalink:  bringing_it_all_together_making_a_ruby_rails_project
---


I did quite a bit of brainstorming for my Rails project. Inspiration struck when I got done playing Dungeons and Dragons with my brother and his friends. I thought "wouldn't it be cool if there was a free RPG character app for this and other tabletop RPGs?" I thought it through and realized it was exactly the sort of thing a logic-based app could do well: organize different universes and define and track traits for characters in those universes. 

I thought it through some more first by considering the model associations that would be used. Characters in a universe are described by different traits. There might be a strength trait in the Dungeons and Dragons universe while in other universes this might be called 'stamina' or be absent altogether. So traits should belong to a universe and multiple characters in that universe. 

But the value for each trait will vary by character. This stumped me for a bit. You can not have a global value for a trait, because that would mean every character in the universe would have that exact value! Some characters are stronger than others, so they should not all have the same strength stat. 

It suddenly hit me: I need a join table! Traits have many characters, and characters have many traits, and there needs to be a stat modifier for just that character and that specific trait just of that character. So the join model is character_traits, which defines a certain character id and trait id and a stat that is the value for the trait for that character. 

I looked through the project requirements again and thought "I can definitely make a join table and nested resources. I can do this." So I made a new github repo and got to work. 

The migrations were the relatively easier part. But I quickly learned the need to constantly refactor as new features were added. I decided to add the Devise gem, and oops there goes the User model! Need to redo that one. Then I wanted omniauth-facebook; oops, need to redo the user model again! 

Google was my best friend during this project. One weakness I have had is trying so hard and stubbornely to figure things out 'myself' when just googling it can give solutions. Combining Devise and omniauth is challenging, and luckily googling that produced a guide for doing exactly that. 

There were a lot of moments where I had to review lessons and google solutions. Nested forms was definitely one such case. I had a use case of nested models, partials, and form_for, which combined made it very tough to find an exact solution through googling. But googling often pointed me in the right direction. A combination of reading, asking on Slack, and trial and error eventually led me to get the nesting correct. 

I learned a ton from this project! What seemed like separate pieces of coding knowledge all came together nicely. My app, rpgsmash, seems to be working well. It is very extensible as well and I plan on adding a lot of features and seeing what my brother and his friends think of it. Programming is a fun challenge that seems to fit my personality to a tee!
