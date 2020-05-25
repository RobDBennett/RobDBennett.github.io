---
layout: post
title: First Build! Steam Data!
subtitle: What makes a game successful on Steam? by Rob Bennett
cover-img: /assets/img/steam.jpg
tags: [builds, blog]
---
<insert header- Defining the Question>
So what makes a game successful on Steam? There are a lot of ways to define 'success', so for now lets focus on how often a game is purchased, downloaded and played.

<insert header- Exploring the Question>
I'm not sure how much of the population is like me. I've lost track of the number of times where I've loaded up Steam, extremely bored, and started flipping through their splash page of 'PLEASE DOWNLOAD ME!' games. There's almost always a sale. Something catches my eye, I click on it. The game looks interesting, I check the price, I argue with myself. I make some very compelling points, and I treat myself to a new game. And yet, after installing the game, I'll sink maybe two to five hours into it before losing interest and sacking it for a return to my old classics. I mean, I have to be an aberrant, right? I'm the guy that has like five-thousand hours tied up in the Civilization series.
Well, lets sooth my suddenly rising concerns that I'm alone in this.

<insert header- The Data>
After poking around for a bit, I found a few data sets that had more or less everything I needed to write a compelling point about my own habits. The first <figure out how to hyperlink- https://www.kaggle.com/tamber/steam-video-games > is a break-down of a sampling for 200k Steam users, new games they bought, and how many hours they spent playing the titles. The other next dataset was here <figure out how to hyperlink -https://www.kaggle.com/nikdavis/steam-store-games > and it had a wealth of data, like the price of the title, some review data, release dates, and the genres tags from Steam.

<insert header- Shaping the Data>
My shaping and visualization notebook can be found here <insert hyperlink- https://github.com/RobDBennett/DS-Unit-1-Build/blob/master/SteamDataShaping.ipynb > for those wanting to follow-along at home. Our first dataset was pretty clean already. There was an extra column, which was dropped easy enough. The second dataset was a bit more clunky with a lot of data that I don't need. I shave off a few of the items that I don't particularly care about for this exploration (like publisher and platform data). 
