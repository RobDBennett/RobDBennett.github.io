---
layout: post
title: Basic Data Science- Linear Models and Applied Modeling
subtitle: The episode where we cover the basics of predictive models! by Rob Bennett
cover-img: /assets/img/Python_icon.png
tags: [unit_review, blog]
comments: true
---

## Overview-
This was the first unit that felt like actual data science. Or proto-data science. We learned to love sklearn (or scikit-learn). This unit also had us move away from Google colabs into local enviornments. There were a lot of interesting challenges to be had with that.
Primarily, we were learning basic linear models to do basic regression and classification problems, and then apply them with toy datasets into something interesting. 

## Sprint 1- Linear Models
LinearRegression, RidgeRegression, LogisticRegression were all the order of the day. They all operate a little differently and are good for different problems. We learned how to do Linear Regression without the help of the sklearn libraries initially and then moved on to more advanced deployment.
Overall, I'd say that Ridge is a better for me. I tend to prefer categorical problems to regression problems. Covered within this section was also one-hot encoder and ordinal encoders. These seem complicated at first, but they're just a way of parsing out the data in a way that the computer understands better.
Things that I should review- SelectKBest, which is a neat tool that helps with feature selection, and Logistic regression (which seems to operate with a sigmoid like function). 

## Sprint 2- Kaggle Challenge
A deceptive name for this Sprint. All of our daily projects were to further our Kaggle project- which was more accurately predicting which water pumps required replacing in Tanzania. 
Big things that we learned this sprint were pipelines. We used these a lot, and in future units we used pipelines all that time. An understated time saving measure to be sure. We also learned about decision tree/ random forest classifiers and a slew of methods for scoring our models. 
Cross-validation is a method of evaluating hyperparameters and 'tweaking' models, it relies on 'folding' the data across different parameter configurations and comparing accuracy scores. A very cool tool that we used in the future, also more advanced methods. CV is computationally very expensive, so we used it sparingly.
Finally we learned a few classification metrics. Namely the difference between Precision and Recall, and the value of the ROC AUC. We learned how to tweak a model so that it reacts differently (for example, changing you parameters to find a small class more frequently, like fraud among bank users or the like). 

## Sprint 3- Applied Modeling
This sprint had the most practical knowledge. Previously, we were told what methods to use on what problems and why we were being asked to do that, but this sprint was all about evaluating the questions to come up with our own strategies. Very cool, really. 
A lot of this was getting in reps on a theme. Find a dataset. Wrangle data. Choose a model. Build a pipeline. Get results. Tweak parameters. Repeat. Find optimal solutions. I have a feeling this was more 'real world' than previous weeks, and honestly the problem solving aspects of the activities were fun and engaging.
A few new models were introduced to us, like xg-boosting which was immediately popular. It was also very instructive to see what models responded differently to pipeline structure. Which needed scalers or encoders, and which ran better and for what reasons. 
Finally, we were given a few tools to help find the best features, my favorite of which was shap_values. What an amazing tool that takes a single instance in a model and details out all the forces that put it at any given point of prediction.

## Closing Thoughts
This unit made me feel like a real datascientist. Or at least one in training. Our capstone for the unit was a Dash app using plotlyexpress and flask scaffolding to give an interactive way to engage with our model in real-time. Very cool. 
I have since referenced this unit frequently, and a lot of tools we used were very practical in nature.

