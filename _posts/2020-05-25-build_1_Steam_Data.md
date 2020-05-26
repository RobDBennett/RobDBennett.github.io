---
layout: post
title: First Build! Steam Data!
subtitle: What makes a game successful on Steam? by Rob Bennett
cover-img: /assets/img/gm-4e09aa7e-d962-47f5-bfca-93b1f81d581f-steam.jpg
tags: [builds, blog]
---

## Defining the Question
So what makes a game successful on Steam? There are a lot of ways to define 'success', so for now lets focus on how often a game is purchased, downloaded and played.
  

## Exploring the Question
I'm not sure how much of the population is like me. I've lost track of the number of times where I've loaded up Steam, extremely bored, and started flipping through their splash page of 'PLEASE DOWNLOAD ME!' games. There's almost always a sale. Something catches my eye, I click on it. The game looks interesting, I check the price, I argue with myself. I make some very compelling points, and I treat myself to a new game. And yet, after installing the game, I'll sink maybe two to five hours into it before losing interest and sacking it for a return to my old classics. I mean, I have to be an aberrant, right? I'm the guy that has like five-thousand hours tied up in the Civilization series.

Well, lets sooth my suddenly rising concerns that I'm alone in this.


## The Data
After poking around for a bit, I found a few data sets that had more or less everything I needed to write a compelling point about my own habits. The first [dataset](https://www.kaggle.com/tamber/steam-video-games) is a break-down of a sampling for 200k Steam users, new games they bought, and how many hours they spent playing the titles. The other next [dataset](https://www.kaggle.com/nikdavis/steam-store-games) and it had a wealth of data, like the price of the title, some review data, release dates, and the genres tags from Steam.


## Shaping the Data
My shaping and visualization notebook can be found [here](https://github.com/RobDBennett/DS-Unit-1-Build/blob/master/SteamDataShaping.ipynb) for those wanting to follow-along at home. Our first dataset was pretty clean already. There was an extra column, which was dropped easy enough. The second dataset was a bit more clunky with a lot of data that I don't need. I shave off a few of the items that I don't particularly care about for this exploration (like publisher and platform data). I merged the two datasets. The first dataset had some double entries since the play/purchase was a single column and if they played it reported 1.0 hours in the hours played column. Not wanting to confuse things, I filtered out the purchased aspects of this for a new dataframe and then I used that to explore the data a bit.


## Explaining the Data
The first thing that I really noticed was the age of some of these games. Counter-Strike makes it into the top ten based on my filtering, and that game came out in 2000! After several hours of hammering away at these datasets, I was able to refine myself to this clean display: 

![Vis3](/assets/img/Vis3.JPG)

Not the prettiest, I know, but it contains a lot of interest, and at least to me, surprising data. I want to focus on two areas that this information jumped out at me for, and then I want to sum this up with some annidotal thoughts on it. First, lets look at the hours people sunk into these titles.

![Vis1](/assets/img/Vis1.JPG)

First off, notice that every single one of these titles has a *huge* difference between the Mean and Median time spent playing them. When I was first exploring this data, I was just going to go with the Mean as my metric, until I took a closer look at the data. Some players sunk an unbelievable amount of time into these titles. One player in Dota 2 had nearly two-thousand hours in just that game alone! If felt a little jarring, but when you look at the Median player's time in the games, you'll notice that it's a much more uniformed distribution.

The second thing that I want to focus on are the reviews for these games.

![Vis2](/assets/img/Vis2.JPG)

I would have expected there to be a stronger correlation between positive reviews and hours the players invested into the game. While all of these games have a very high percentage of positive to negative reviews, you'll notice that the sheer amount of reviews really drops off the further they are from the #1 slot. 

## Conclussion
My first take-away from this is to breath a huge sigh of relief and realize that I'm not alone in my gaming habits. But back to the question: What makes a game successful on Steam? 

It seems to break down into four major categories. 
1. The title needs to be affordable. Every game in the top ten slot had a sale price of less than $8 dollars. That's bonkers, when you really think about it.
1. It needs to include the 'Action' tag for the Genre. 9/10 of the list included the 'Action' tag.
1. It needs to have a high 'replay' factor. Consider the age of these titles. Half of them weren't even released this decade, and one was released back in 2000. That tells me that there is a mix of nostalgia for sure, but these games also need to have some staying power. This is probably the hardest thing to pin-down, but a lot of these games also have multi-player group v group round style play for quick pick up games.
1. Your title needs to have a lot of positive reviews. Word of mouth seems to be far more effective than advertising dollars. Games that have been out for awhile don't have people spending money to hype them up. They make their own sauce, as it were. If you have a game that people like, that momentum will carry them forward for many years to come.
