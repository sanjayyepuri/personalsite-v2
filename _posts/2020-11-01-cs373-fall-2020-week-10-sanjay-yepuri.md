---
layout: post
title: "CS373 Fall 2020 Week 10 - Sanjay Yepuri"
description: "Week of 26 Oct. - 1 Nov."
category:
tags: []
---
#### What did you do this past week?
This past week our team researched free-text search and filtering. We found a SAAS platform called Algolia that provided a Google-like search experience with data that we provide. Additionally, I made minor UI tweaks cleaning up missed details.

---
#### What's in your way?
I am waiting for our models to be moved to Algolia. Once completed, I will start integrating the search and filtering UI into the model pages.

---
#### What will you do next week?
I need to decide the best way to integrate the search and filtering provided by Algolia. Algolia provides react components that we could use. However, I want to explore other options that we have.

---
#### If you read it, what did you think of The Interface Segregation Principle?
The Interface Segregation Principle outlined common patterns to avoid when design software. In particular, the "fat interfaces" the author mentioned are problems that I have experienced. In a previous internship, I found myself implementing methods to conform to an interface. These methods were never used and only existed to make the code compile. The dispatch and multiple inheritance patterns are solutions that I will keep in mind while designing software.

---
#### What was your experience of instance methods, class methods, static methods, regular expressions, and relational algebra? (this question will vary, week to week)
I have not written a lot of python code with class and static methods. However, I have used instance methods quite regularly. I learned making instance variables private and the differences between class and static methods. I will have to try them out myself before I know when to use them.

---
#### What made you happy this week?
This week I did not have an insane amount of work. I was able to, in a very laid back manner, complete my assignments, and get them turned in.

---
#### What's your pick-of-the-week or tip-of-the-week?
I found an interesting project on Github called [Citybound](https://aeplay.org/citybound). This is a city-building game (similar to Cities Skylines) built in Rust. The author's website details its design and some of the decisions he made. The architecture of the game is designed to be distributed and multithreaded. He also built an actor-system framework he uses to build his city simulation. This project uses a few other interesting concepts, such as incremental computation and using Rust+WASM for the frontend. It is worth taking a look.


<img src="/assets/headshot.jpg">
