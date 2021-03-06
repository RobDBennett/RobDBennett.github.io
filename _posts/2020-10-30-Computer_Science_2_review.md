---
layout: post
title: Exploring Computer Science Principles #2
subtitle: The episode where we cover the more advanced concepts of graphing, hashing, and emulators! by Rob Bennett
cover-img: /assets/img/Computer-Architecture.jpg
tags: [unit_review, blog]
comments: true
---

## Overview-
Unit 2 of Computer Science was harder than the first, and the first was pretty rough at times. Taking the lessons that we learned about data structure, Big O notation regarding space and time complexity, and some logic regarding how computers function, we dove into hashtables (dictionaries, for python users), graphs (not the visual kind), and how to build virtual machines. Some of these concepts were hard to grasp all on their own, and when you look at it through a bird's-eye, this was a lot of material in a very short amount of time.  

## Sprint 1- Hash Tables
This sprint was about introducing us to hashtables. I want to go on record as having known about python dictionaries for a long time. When we were first introduced to them, we were told that they were faster, but not really why. To date, I found myself enjoying arrays far more than dictionaries. However, after being introduced to how hashing functions work, and how space/time efficient they are compared to arrays, I don't think I'm ever going back. I think that hard part, at least for me, to grok was how repeatedly we were told that hash tables search faster. The reality is that they do very little searching at all. You have a function that renders and input to a predictable number, and that's the address for that thing. Wild concept, really.
We built several hashtables from scratch to understand how dictionaries work. Concepts that had previously been known to be, like dictionaries within dictionaries, and how to call the element of an element of an element were used repeatedly. Being able to look at a logic problem and know its a hash problem has proven to be very powerful for things like LeetCode challenges.

## Sprint 2- Graphing
Graphing, as used here, is more like linked lists or binary search trees than about bar graphs and pie charts. Basically, its a digital representation of space. You have a collection of nodes that might represent any number of things. They have values associated with them, or strings or, anything really. Then the nodes are connected to one another either one way or two way, and these connections (called edges) might have values associated with them too. This is how you might draw out a map, or a logic puzzle. None of these concepts are individually difficult, but they also aren't super simple. Figuring out how to tranverse a graph is similar to binary search trees. Depth First or Breadth First tranversal or searches have wildly different results. Once you understand how they operate, and what code you need to tweek to make it do one or the other, you have a much easier time understanding graphs and their power within computer science.

## Sprint 3- Computer Architecture 
This sprint was very difficult to understand. It started off fairly simple. We broke down how computers actually operate, which is stuff that all of us at least sort of understand superficially. A series of switches, is how I thought about it. Now I understand its a series of transistors on a chip that act as switches with voltage rather than physical switches. We then broke down how CPUs operate (not in depth, they have gotten really complicated).

![CPU](/assets/img/Block-diagram.jpeg)

With some high brow concepts under our belt, we dove into building a virtual 8-bit CPU using pure python. Using assembly language, we wrote programs (which was, point of fact, considerably more difficult than the python coding). What I really enjoyed about this was the logic of it. Assembly language really forces you to think about what bit and byte you need, and how many registers or units of ram you need to execute basic stuff. We build up the ALU (the logic unit that handles math) with various functions like basic math and higher concepts like XOR and their like. The hardest part, at least for me, was trying to get things like timing or keyboard interrupts to work. I can say with a fair degree of confidence that I understand how computers physically operate much better than before. 

## Sprint 4- Build Week
Normally I give build's their own post, however, this build week is a bit misleading. This entire sprint was interview preparation. From resume polishing to whiteboarding challenges, from conceptual interview questions to actual fake interviews, the name of the game is getting job ready. This week was also our final unit assessments and the General Coding Assessment. I'm not going to lie, the GCA was brutal. You are timed, recorded via webcam, your screens are recorded, and your test time is reviewed. You aren't allowed to search for any answers at all. I've never, in my time in Lambda, felt so helpless. We become reliant on searching rather than memorization. Overall, I feel that understanding concepts and how to ask questions is a more powerful survival tool rather than rote memory. Until you're tested in this way, or have an interview where you can't ask Google for a refresher. This stuff was very hard.

## Closing Thoughts
The Computer Science units in Lambda were hard. I mean, really hard. The Data Science track had some challenges, like Object Oriented Programing, or just the speed that concepts are thrown at you and expected to be assimilated. With Computer Science, it's all of the same stress with the added bonus of adding higher end programing to the mix. Between the algorithms and the breakdown of things that python does natively, there is a lot to unpack here. The hardest parts of the unit was the emulator, the GCA, and some of the graphing concepts. Its hard to retain everything that you need to remember and know, and have immediate recall on it. The whiteboarding interview questions were actually fun (most of the time), though some of the harder ones were stressful. Best advice that I can give here is to talk out-loud, treat the whole room like your rubber ducky, and don't feel too bad about sounding stupid. 
