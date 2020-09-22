---
layout: post
title: Build 4- Saltiest HackerNews
subtitle: Can we identify 'salty' commenters on HackerNews? by Rob Bennett
cover-img: /assets/img/hackernews.png
tags: [builds, blog]
comments: true
---

## Overview-
This was our second group build, with cross over from the web team. The goal of the project was to take in data about the Hacker News website, evaluate the relative negativity of the comments each commenter made, assign them a negative value and the commenter an overall negative value. 
This was another project that was a little tricky. We had some API difficulties and ended up going with a saved dataset that was a few years old. The team also had some difficulties. The first day in, we lost our back end developer to a flex, and the Lead for the project had to step in. Unfortunately, this caused her focus to shift, and the front end team never hit MVP. They didn't even deploy a website, so I can't include a completed project for you since it was never finished.

## Sourcing the Data
Our data was a few years old, but with 700+megs of information, there was quite a large collection of commentors and their posts. The data was fairly clean to start, but it did include a lot of things that weren't necessary, like links to articles and what have you. We tried with a few lighter weight sets, but at the end of the day, this was the one to go with.

Our source data can be found here: https://zenodo.org/record/45901#.X2p4N2hKiUl

## Exploring the Data
In order to get the data ready for NLP, we had to do a lot of streamlining. We cut down a lot of columns, tokenized and pulled stop words. We tried a method via beautiful soup that allowed us to keep emojis, but it ended up performing a little worse than just straight nltk. The process only took a few hours, but the whole team jumped on it and that was a good thing to see. While the rest of the team was a bit soft, the DS team was solid. 

## Model
We tried a few different models here. We deployed a Vader model, built a neural network with tensorflow from scratch, but ultimately ended up going with nltk, with a NaiveBayesClassifier. Once the corpus and stopwords were formed up, we put the comments through a Lemmatizer (finding it did better than straight tokenizing), and then applied the model to the cleaned data. The performance was reasonable, though things like sarcasm are hard to pull out, and typos caused some data loss. Anything that involves 10k+ end users is bound to be full of difficult to uniform text. 

## The DS App
The DS team put together a RapidApi app with some prebuilt scaffolding. It was able to allow you input a user and get their comments, select most salty and get a list of salty commentors, or look for salty comments in general. While some of the formatting can be difficult to weed through if you pick a high number, the speed that it operates is truly impressive. It took the whole team about three days to get the model properly wired in, with a near constant Zoom call going. Sometimes I think it would have been easier to just do this project solo, but having a lot of input definitely made this project feel very rich!

Our DS app can be found here: https://saltiest-hacker-news.herokuapp.com/#/default/get_comments_comments__get

## Closing Thoughts
This was a tricky project. It doesn't feel great to invest a lot of time into a project just to have it not fully deploy. The DS team hit all their marks, and hit them early (though not impressively early). Overall, this was a good learning experience to understand just what it would feel like to be attached to a team that wasn't quite succeeding, even though you personally are. Its a tricky feeling and I was quite ambivalent about it. 

Our repo can be found here: https://github.com/bw-saltiest-hacker-1/DS
