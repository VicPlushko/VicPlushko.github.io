---
layout: post
title:      "My Rails Project"
date:       2020-09-14 07:10:19 +0000
permalink:  my_rails_project
---


All I can say is that this project was a struggle. One of my problems was the has_many through assosiation. I spent all of 2 days working on getting my models to associate right. My next struggle was with the OAuth requirement. I learned a very valuable lesson during that process and that was to make sure and look at the log in my terminal when I am having trouble getting something to work. I spent the better part of 10 hours trying to get a Facebook login setup, then after hours of getting close and felling like i was beating my head against a wall I decided to go with a oauth for GitHub. Even that process had it's moment of torment, until that fateful time that I looked at my terminal and just as clear as day it was telling me what was wrong. ONE LINE OF CODE!!!! "before_action :user_logged_in" this method was not allowing github to route to the proper place because this method was redirecting to the root route for my app.

Other than being stuck on two problems for a day a piece, I did learn alot. Some of the concepts that I struggled with during lessons in the Rails Mod  became more clear to me, for instance figuring out what variable (@herb vs herb) to put in whatever path that I was redirecting to or linking to. Working with forms definitely got much easier during the project. I enjoyed the challenges that this project presented. I had my first experience with having to make migration after migration to keep changing something in my database tables. I think I made 4 migrations back to back to add some columns to users table just to turn around and get rid of those columns about 30 minutes later. It always made me chuckle everytime I realized that I needed to make yet another migration.

So overall this was a fun yet frustrating project for me, but it has left me wanting to really dive into RoR and to expand this projects features and make this app as good as I can possibly make it.


