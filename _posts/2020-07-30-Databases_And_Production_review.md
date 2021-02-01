---
layout: post
title: Intermediate Data Science Review- Databases and OOP
subtitle: The episode where we cover the basics of OOP and databases! by Rob Bennett
cover-img: /assets/img/Python_icon.png
tags: [unit_review, blog]
comments: true
---

## Overview-
This unit was the most difficult in Lambda to date. Object oriented programming comes out of left field and you have a very short period of time to familiarize yourself and get your feet under you before you are producing functional code. Very tricky stuff. We moved from that into databases and some other sundry stuff. While SQL was something I had some previous experience with, it was neat seeing how we could take vast data from structured databases and force ML algorithms onto them.  

## Sprint 1- Software Engineering and Reproducible Research
I'd place this Sprint in the top three hardest weeks of the course. In broad strokes, we covered OOP, containers, and how to build packages. We also covered how to form enviornments for testing, though I had done a good deal of that in Unit2 as a stretch on the build week. There was a lot of good things here. Building classes in Python proved to be wildly powerful. Though it was hard to wrap your head around. We built and publishes a python library that we can download and access later. Very cool. Also, we covered a great deal on licensing, focusing largely on the MIT license. Most of this unit was treated as something of a footnote with the clear focus being on classes and object oriented programming. Also covered was unittest, which I also feel didn't get nearly enough attention. I wrote several, but likely need to get more reps in. This was a simple concept that I had some difficulty implementing. Given the scope of the data and speed that you have to process it, compared to other Units this week felt like a *whole* unit unto itself.
I should probably brush up on Docker a bit more.

## Sprint 2- SQL and Databases
This sprint was a much easier time. SQL is familiar to me and the queries are simple and intuitive. There are inner/outer join problems that you need to sometimes try different ways, but there are a host of online tools to brush up on a moment's notice. We covered sqlite3 for python, as well as postgres particularly as it related to a Heroku deployment. There was some introduction to NOSQL and Mongo style databases, which feel very powerful but prone to chaos. We addressed a lot of schema issues, but didn't go into as much depth as we could have. The goal here isn't to become architect level, but rather conversational on the topic and different scopes we have. ACID was a big concern as we moved away from SQL. How an entry is accessed and updated, security and sanitization were also covered to some degree.

## Sprint 3- Productization and Cloud
This sprint was all about apps and api's. We built several heroku apps that did little things. For instance, we built an app that interfaced with Twitter. You downloaded the tweets from various people, and then trained a ML model which then predicted who would have said a new tweet based on the people you had trained it to recognize. This could get a little out of pocket, depending on how verbose the users you chose to include were. However, sliding heroku into a postgres database and then updating that database with an api was all incredibly powerful. Not all api's are created equally though, and we had some trouble interfacing with other sources (like HackerNews). This was also our introduction to Flask, which I had a leg up on since I had done a Dash app in unit 2 (dash being constructed using flask, they are pretty similiar). Our sprint challenge was with openaq, which measures air quality at various cities around the globe and reports the different findings back. Very cool stuff, and felt very real-world appropriate. A lot the data that we have dealt with till now was toy models, so pulling in functional data via an api was a step in the right direction.

## Closing Thoughts
This was a very challenging Unit. All and all, I learned a great deal, and I got in some good reps. APIs and Docker could probably use a brush up. The concepts of pipenv and the like were also very powerful. It hits a point that you often just forget what libraries you have installed on your machine, and you take them for granted. So developing tools to avoid the 'well it works on my laptop' problem was very neat. Also, simple ways to deploy low-energy apps to display the data you have collected and the results is also very cool. 
