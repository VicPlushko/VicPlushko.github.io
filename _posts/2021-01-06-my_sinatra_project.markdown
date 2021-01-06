---
layout: post
title:      "My Sinatra Project"
date:       2021-01-06 14:55:18 +0000
permalink:  my_sinatra_project
---


Getting to implement the things that I learned about Sinatra, C.R.U.D and RESTFUL routes was a lot of fun. I have to admit that learning about routes and views was a challenge for me. There were some things that I just didn’t get at first. It also seemed to me that at times I was fretting about things that in the end boiled down to convention. One instance of this was figuring out the naming convention for get and post routes. It threw me for a loop, I don’t know why, that a route was get ‘/dogs’ or post ‘/dogs’. In my head I obsessed over where that name was coming from. I eventually got the hang of it and everything began to smooth out.

One of the challenges that I had with this project was getting my search bar to function like I wanted it to. When I got the code for my search method correct in my model, well, it was correct in the sense that my search page would actually perform a search and render my results view. When I got the search function to function I could only search by name. 

ex:

def self.search(search)

where(“name LIKE ?”, “%#{search}%”)

end

I tried changing name to taste and I was able to search by taste but not name. As I had 5 different properties that I wanted the user to be able to search for I began to rack my brain and google for a solution. As I was looking at the time and noticing that I had to go get ready for work, I all of a sudden thought about using the ‘or’ operator ‘||’ and so I tried this bit 
of code…

def self.search(search)

where(“name || taste || energetics || actions || ideal_for LIKE ?”, “%#{search}%”)

end

and voila, I was able to search by all five of the properties that I wanted to search for. This was a throw my hands in the air and dance around kind of moment for me, it felt so good to have thought of the solution to this problem, especially right before I had to go to work.

During this project I learned a lot more about HTML and CSS. I got to learn more about CSS selector and even how to do some styling right in the html code.

Over all it was super fun to watch a web page come to life piece by piece. It certainly gives you a sense of accomplishment when you sit back and look at your web app and see how far it has come.
