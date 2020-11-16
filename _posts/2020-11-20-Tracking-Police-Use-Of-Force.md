---
layout: post
title: Labs! Tracking Police use of Force!
subtitle: How can we best hold the watchmen accountable? by Rob Bennett
cover-img: /assets/img/human-rights-first-dark.png
tags: [builds, blog]
comments: true
---

## Defining the Question
What is the best way to hold policing organizations responsible for what they do? What is the best way to keep the public informed of these actions? More now than ever in American history, we have a spotlight on police over-reach and a rising sense of disquiet from the general public.


## The Organization
One of the leaders fighting for transparency is the Human Rights First organization. They have been around for nearly 40 years fighting for equality and fair treatment under the law. They have an extensive history in defending minorities, combating torture, and ensuring consistent respect for human rights. They are a non-profit, nonpartisan international human rights organization primarily based out of New York, Washington D.C., Houston and Los Angeles.

Their Chief Technology Officer approached my team to workshop a solution to a lack of transparency on these topics.

More information can be found on this fine organization on their website, located below.
[Human Rights First](https://www.humanrightsfirst.org/)


## Understanding the Problem
On its surface, this seems like a straightforward problem. The reality is anything but. The laws that dictate how a policing organization self-report can vary wildly from County to County and State to State. The FBI has formed a group dedicated to monitoring police use of force, but unfortunately, they don't have the legislation in place to demand compliance. They are only allowed to ask the various police organization to participate in their metrics, and only around 50% of them have elected to join.

![ufo_participation](/assets/img/uof_participation.JPG)

More information can be found here: [FBI Use of Force Collection](https://crime-data-explorer.fr.cloud.gov/officers/national/united-states/uof)

In the absence of any effective government oversight on this troubling descent into a police state, we the people need to report and hold these organizations accountable. Getting this information is tricky in the best of times. Various news outlets and watchdog groups do what they can to keep tabs and report, but it simply isn't enough, and it is too scattered. It is difficult to sort through, and hard to grab a snap-shot of these incidents. 

The problem that we struggled with throughout this project was lack of data or transparency. Until we have a central voice of truth on this matter, we are largely forced to engage social media to find details about these things. Often times these can be from primary sources, but social media also opens us up to falsely generated news or re-tweets that are months old.


## Our Solution
Using a variety of sources, ranging from the Washington Post, to the police brutality tags in twitter and reddit, we built a robust pipeline of data through which we could generate clear visualizations and some interactive graphs.

[Police_Violence_Tracker](https://d-fe.humanrightsfirst.dev/)

The goal here is to have a single location that draws from multiple sources and compiles in a logical manner. The graphs are largely interactive, and a range of filters give end users many options on how best to engage this data. We were able to find a good deal of historical data on lethal police encounters, but there was are much less accurate reports of less than lethal police encounters. Tear gas, presence, tasering (that doesn't lead to shooting) and other forms of chemical force is less well tracked. For this we turned to social media, specifically the subreddit regarding police brutality, and some twitter. These are easy to access using the 2020PB API.


## Concerns and Fears To Overcome
Outside of this project, I had concerns regarding the wealth of data that we could find. I had written a police-shootings app a few months back, and so this was not a new struggle for me. The complete lack of transparency is extremely troubling. The social ramifications are also difficult to fully 'grok'. As a majority class person, it is difficult to understand the minority, and projects like these run the risk of being tone-deaf 

For the project itself, I had some concerns with working with a different devotion of programming, as well as a few of the elements necessary to properly execute this project. Docker, AWS, and database architecture. These were technologies I learned a few months ago, so I was worried about being a bit rusty. Docker had been a challenge to implement correctly with the virtual machine memory, but once WSL2 was properly running, everything else was fine. AWS is also an extremely user-friendly product for Elastic Beanstalk and RDS. 

As far as my concerns regarding working with the team, it was mostly surrounded by not knowing the other actors involved. Fortunately, I was very familiar with my partner on the Data Science team. All of these problems were made better by engaging them. The team was immediately less intimidating after our first meeting. My concerns Docker or AWS were resolved by reading documentation and working through various help files. The only real concern that persisted beyond the first few days was data sourcing. There just isn't much out there.


## The Product Roadmap
We began this project by having a meeting with the stakeholder to see what some expectations were and what previous groups had difficulty with. Dr. Chang was extremely knowledgable on our topic, and as a data scientist himself, he was very familiar with the problems that we were facing. Taking his expectations to mind, we then fell back into our groups to discuss further.

We generated a Trello board and began to populate it with user-stories, most of which were taken directly from the stakeholder's vision. These cards were then fleshed out with a checklist of necessary steps that each would require before they could be considered finished. The various teams were assigned to the tiles, and for those who felt particular inspiration, individuals were joined as well. Trello has proven to be an immense resource, not just with this project, but many of the side projects I have worked on in recent years.

![trello_card](/assets/img/trello_card.JPG)

The above Trello card is the meat of the project. It involves all of the teams and requires other tasks to be done. It tracks the proper chain of custody on the data to the end user. In the description we put a helpful link to help Front-End learn about the technology we were going to use to execute this task. And below we had space to keep each other updated when various tasks were completed as well as moving the tile along through the process.

Once we had our vision, expectations, and list of user-stories populated, we built a wire frame to outline the architecture of this project. The frame itself is fairly expansive, but I have included the Data Science team's frame. Note that all of this was done before any actual coding took place, or before we began searching for primary sources for our dataframes. Not all of these elements made it into final production. 

![wireframe](/assets/img/DS_Wire_Frame.JPG)

The above details the work-flow for the Data Science team, along with all of the potential aspects of the project that we might be able to develop. Some elements we didn't have time for, or we didn't find proper sourcing (such is the case for the FBI database), others didn't prove fruitful such as the NLP model. The majority of these bullpoints were utilized in our product, however, and they are factual for this framework. This proved an excellent reference tool for all of the various teams. It was most utilized by the Backend Developer, which is where you can see the line going off camera.


## Specific Work and Technical Challenges
Words.
![code_snippet](/assets/img/HRF_Code_Snippet.JPG)


## Problems the rest of the team suffered



## The Project As of Now



## The Future of the Project



## Final Reflections

