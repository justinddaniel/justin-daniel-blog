---
layout: post
title:      "Building a Sinatra Application (Swap-your-Stuff)"
date:       2017-11-03 18:16:51 +0000
permalink:  building_a_sinatra_application_swap-your-stuff
---


I just finished the first iteration of my Sinatra Project and had a lot of fun building it! It was fun brainstorming and coming up with something I think is useful, and then building it from start to finish. My app is called Swap-your-Stuff, which serves dual functionality. It allows users to keep an inventory of all of their belongings and then, at their choosing, select which items to make publicly viewable for selling/trading. 

I could clearly see how what I learned with CRUD routes helped clarify my thinking and gave me clear patterns I could use when coding. I needed to create a homepage, a user inventory page, a form for creating new items, and routes to edit and delete these items that only the user who created the items could utilize. I also had to make sure that sessions were used to make it a pratical application, and that passwords were secure. Seeing all of this knowledge I spent the past 3 weeks acquiring come together was really gratifying!

The one major roadblock I ran into was how to edit a Boolean type of data with an edit/patch request. Apparently ActiveRecord does not allow a simple .= method for editing a Boolean in this manner. I tried googling around to no avail. I credit the slack community for giving me an outlet to share the problem and some brilliant member came up with the solution of using .update_attributes(attribute: value). This was a good lesson that belonging to a community and reaching out to them is important, because google can not solve all of your problems!

I really look forward to the next project and applying some more programming knowledge!
