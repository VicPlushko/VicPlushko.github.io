---
layout: post
title:      "My Adventures in JS"
date:       2020-11-09 00:54:43 -0500
permalink:  my_adventures_in_js
---


My mod 4 project for Flatiron School was certainly an experience. It also gave me some great experience into the world of Javascript and using JS to do everything without reloading the web page. There were a few key moments during this build that helped clear up alot of the questions that I had or the concepts that I struggled with during the mod 4 cirriculum.

To begin, using Javascript, some starter HTML and CSS to create the client side of this web app was a little intimidating at first. The experince of having to plan out what I wanted on the page at any given moment was really cool and at times really frustrating. Getting that first bit of data back from my first fetch was real satisfying, then I needed to figure out how to get that data to display the way that I wanted. In the case of my project I have 5 different sections each containing a div and a ul. My first hurdle here was to figure out how to sort the tasks that I had previously made into the proper divs. My solution was as follows 

       `allTasks.forEach(task => {
            
            const taskInstance = new Task(task)
           
            if (task.routine === "Morning") {
            morningUl.innerHTML += taskInstance.renderTask()
           } else if (task.routine === "Homework") {
               homeworkUl.innerHTML += taskInstance.renderTask()
           } else if (task.routine === "Chore") {
               choresUl.innerHTML += taskInstance.renderTask()
           } else if (task.routine === "Bedtime") {
               bedtimeUl.innerHTML += taskInstance.renderTask()
           } else if (task.routine === "") {
               miscUl.innerHTML += taskInstance.renderTask()
           }
       });`

Getting past this first hurdle helped me alot during the rest of this build as most of the time that I needed to display something I had to use a similar method to accomplish what I needed.

Adding event handlers to links and buttons. This was something else that caused a bit of frustration. There were times when I would click on a link or a button that was on the page and absolutely nothing would happen. After a few moments of dread and despair, I would remember that I need to give that link or button some kind of functionality. Enter addEventListener(), after passing in the callback function and then writing that callback function, it was such an awesome feeling to see those same lifeless links and buttons start to function.

This project like all of the prior ones has helped me to learn to pay attention to detail. More so with this JavaScript project. I can't count how many times I sat there frustrated for 20 minutes because I was missing an "r" or an closing "}". The more I experienced the error codes that came along with these mistakes, usually "can not read "some property" of undefined", I was able to find my problem more quickly than the time before.

Over all this was a fantastic experience and I thouroughly enjoyed building this project. I had my ups and downs but in the end I learned alot and that JavaScript code I read on StackOverflow during my Rails project makes more sense now. I look forward to the next mod and getting to make another project in Javascript.
			 
			 
