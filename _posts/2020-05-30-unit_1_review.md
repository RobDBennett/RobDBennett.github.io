---
layout: post
title: DS-Unit 1 Review
subtitle: The episode where we cover the basics! by Rob Bennett
cover-img: /assets/img/Python_icon.png
tags: [unit_review, blog]
comments: true
---

## Overview-
The start of a new thing is always a stressful time. The first unit of Lambda was perhaps among the most nerve-wracking of my life. A lot of changes all happening at once. Juggling a baby and household while also finding the time to learn code was very challenging. Aside from some growing pains though, this unit wasn't terribly difficult. 
We covered a lot of basic material. Sprint 1 was all about data wrangling, cleaning and figuring out how to make it tell you something. Sprint 2 was statistics and Sprint 3 was linear algebra. 
  

## Sprint 1- Data Wrangling
Data wrangling is the subtle art of taking some sort of dataset and turning it into something manageable. In python we use the pandas library pretty extensively here. Also covered in this section were the making of functions and basic for loops. Honestly, I think this course could have benefitted from a more prolonged introduction to the language, but hey, we work with what we have.
Python has a number of tools hardboiled into the system that allow for data to be played with and modified more easily. But most of the things you will do will be functions you make yourself. Since each dataset is different, each has a different 'dirty' element. Sometimes you have extra punctuation or strings, sometimes you have white space, sometimes you have things in the wrong columns or the types incorrect. Understanding how to construct your functions to clean your data is very important. With a bit of hindsight, this sprint has proven to provide some of the tools that we use more than any other tool. 
The last part of this sprint was basic visualizations. This is still something that I need to work on a bit. Plotlyexpress, matplotlib and seaborn are all excellent tools. I am expecting that in the actual field, I will adopt whatever my employer wants me to use.


## Sprint 2- Statistics
I have to say, I remember stats being a beast in college. With python, though, this is a dream. What I love about stats is that they are all word problems and logic problems. The differences between Frequentist and Bayesian statistics is pretty fun to explore. I enjoy how you need to explore the question before really answering it. 
For this sprint, we focused on a few different equations, most of which were found in the scipy.stats library. This library, as an aside, is very powerful and made a lot of those things that I remember making me cry years ago, rather simple to implement. 
Our primary focus was on running T-Tests, Chi^2 tests, and understanding Bayesian things. Chi^2 tests require the use of crosstabs, so  you need to arrange your data appropriately. Then you can run the stats.chi2_contingency commands. 
T-tests rely on stats.ttest_ind commands, and its pretty simple. 


## Sprint 3- Linear Algebra
Linear algebra is all about vectors. Vectors for days and days. My big take-away from this sprint is that the 3blue-1brown videos are amazing. Also, matrix work is far easier with the numpy linalg library. This stuff was the bane of my existence in high school and early college. I barely made it through; the repeatative calculations were tough. But with the help of python, its a breeze now. 
We went through a lot of things unit, but the hardest to keep track of was all of the different notation. There is *a lot* of notation for linear algebra. Things to remember- a little arrow over a variable means its a vector. A big E references a matrix (or any letter), with -1 and T meaning invert and transpose. Havine solid lines surrounding a big letter means the determinant (which determines if its invertable). The Eigenvalues and Eigenvectors are vectors that change in the least way for a given transformation and don't change their orientation, where Eigenvalues are the magnitude of change on those vectors. 
Also covered in this section were PCA and Clustering, which are both very important to understanding machine learning algorithms. PCA being principle component analysis, typically found with the PCA command, which needs to be fit usually compares PC1 to PC2 and so forth. Clustering is a simple method of machine learning that relies on Euclidean distances to determine how similar a given values is to each other.


## Closing Thoughts
In many ways, this was the most challenging unit. We didn't cover as much code as we do in future units, but the raw concepts we go over are legion. You have a week to refamilizing yourself with Stats, a week to understand and deploy linear algebra, and a week to figure out all of the basics of python and data stream-lining so that you will be able to run different ML programs on your data in the future. 
There are many elements of this unit that I will no doubt have to review in the coming months, and I will keep all of my notebooks handy for on the job references!

