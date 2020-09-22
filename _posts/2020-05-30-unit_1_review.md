---
layout: post
title: DS-Unit 1 Review
subtitle: The episode where we cover the basics! by Rob Bennett
cover-img: /assets/img/Python_icon.png
tags: [unit_review, blog]
comments: true
---

## Overview-
So what makes a game successful on Steam? There are a lot of ways to define 'success', so for now let's focus on how many hours players sink into their titles.
  

## Sprint 1
I'm not sure how much of the population is like me. I've lost track of the number of times where I've loaded up Steam, extremely bored, and started flipping through their splash page of 'PLEASE DOWNLOAD ME!' games. There's almost always a sale. Something catches my eye, I click on it. The game looks interesting, I check the price, I argue with myself. I make some very compelling points, and I treat myself to a new game. And yet, after installing the game, I'll sink maybe two to five hours into it before losing interest and sacking it for a return to my old classics. I mean, I have to be an aberrant, right? I'm the guy that has like five-thousand hours tied up in the Civilization series.

Well, let's sooth my suddenly rising concerns that I'm alone in this.


## Sprint 2
After poking around for a bit, I found a few data sets that had more or less everything I needed to write a compelling point about my own habits. The first [dataset](https://www.kaggle.com/tamber/steam-video-games) is a break-down of a sampling for 200k Steam users, new games they bought, and how many hours they spent playing the titles. The other next [dataset](https://www.kaggle.com/nikdavis/steam-store-games) and it had a wealth of data, like the price of the title, some review data, release dates, and the genres tags from Steam.


## Sprint 3
My shaping and visualization notebook can be found [here](https://github.com/RobDBennett/DS-Unit-1-Build/blob/master/SteamDataVisualization.ipynb) for those wanting to follow-along at home. Our first dataset was pretty clean already. There was an extra column, which was dropped easy enough. The second dataset was a bit more clunky with a lot of data that I don't need. I shave off a few of the items that I don't particularly care about for this exploration (like publisher and platform data). I merged the two datasets. The first dataset had some double entries since the play/purchase was a single column and if they played it reported 1.0 hours in the hours played column. 

Then I did a hard look at the data again and found some very big errors that were going to taint my results. Many of the game titles hadn't translated corrected due to minor differences between the two sets of data. Primarily this was around sequel-like titles that included punctuation differences, or trademark style symbols like in the Call of Duty or Civilization series titles. I spent a few hours going through the top 30 games from the first data set to ensure that the metrics that I wanted were clear. While there was a sizeable portion of data lost, this was mostly for minor titles, and nothing in the top 20, which is where I was focusing my efforts anyway. Not wanting to confuse things further, I also filtered out the purchased aspects of this for a new dataframe and then I explored the data a bit.


## Closing Thoughts
