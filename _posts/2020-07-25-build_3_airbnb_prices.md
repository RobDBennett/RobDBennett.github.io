---
layout: post
title: Build 3- AirBNB Price Maximizing!
subtitle: How can we maximize the listing price for an AirBnB stay? by Rob Bennett
cover-img: /assets/img/Python_icon.png
tags: [build, blog]
comments: true
---

## Overview-
The Unit-3 build was our first team building project with Lambda School. The Web students start group builds in Unit 1, so they have a lot more cross-over. This was a challenging experience because you have a week to get a project that you probably aren't that excited about off the ground, and learn how about 15 people operate as well. There are some benchmarks you need to hit, and well laid out milestones, but I still wouldn't call this an easy thing. 
Our project was to maximize the listing price of a given AirBnB location. The locations were made by the user, and a ML algorithm should spit out a prediction on what the maximum price should be.

The final project can be found here: https://buildweek.netlify.app/
  

## Sourcing the Data
At the time of this project, AirBnB had shut down their API so getting fresh data was tricky. They have been having some concerns about Covid, and I imagine their business has been slowing down a bit because of the lack of travel. We went to Inside AirBnB for our data.

http://insideairbnb.com/get-the-data.html

## Exploring the Data
This data was incredibly dirty. Most of it was web-scrapped. Often the columns didn't match up, or the contents were wrong. Because so many things were entered by hundreds of end users, it was all over the place as far as uniformity goes. We were able to pick about 30 columns to fix, but even that was dicy. The benefit of these datasets is that they encompassed much of the globe, so they had stuff all over the place. 
For our app we focused on the US and trimmed down as much as we could. The cleaned dataset still represented nearly 300mgs which was enough to slow our app deployment down considerably. 

## Model
The DS team elected to use a neural network for this problem. There were likely simpler models that would have performed as well, but they had just studied TensorFlow and wanted to flex their muscles a bit. I wasn't privy to most of the details as I was on the app side of things, but I watched some of their training and it was very exciting. 

## The DS App
For the DS side of things, we went with a Flask app. It was very simple, but I learned a great deal. As a for instance, did you know that Heroku doesn't support all version of TensorFlow? I didn't. Did you know that you have a lot of trouble using pipenv with TensorFlow when its not supported? I didn't. This was a learning experience all around. I had to continually get with the rest of the DS team to figure out their versions of things before updating my requirements.txt file so that Heroku would deploy correctly. 
This was also my first time working with TensorFlow, and getting it wired into my app was a little tricky since I hadn't been trained on how the model worked or spat out outputs either. It wasn't terribly challenging, but was *really* eye opening for what this unit had covered with dockers, pipenv, and having something work on your machine, but no one elses.

Our app can be found here: https://ds-bw-airbnb-2.herokuapp.com/

## Closing Thoughts
The cross functionality of web students and DS students was great. I got to see React in action a bit, though I didn't work with it much. It became very clear to me that they spoke almost another language, those web students. Previously I had thought that a software engineer wouldn't be viable if they weren't fluent it most coding languages, but it's been a long time since I was learning this stuff and now there are so many languages that seems impossible. Its all about quickly understanding syntax and getting some cross over on what the rest of the team needs. A very rewarding project.

Our repo can be found here: https://github.com/Build-Week-Airbnb-2/DS
