---
layout: post
title: "CS373 Fall 2020 Week 8 - Sanjay Yepuri"
description: "Week of 12 Oct. - 18 Oct."
category:
tags: []
---
#### What did you do this past week?
This past week for SWE, I focused on building out some local development infrastructure. I added a docker-compose file that will spin up both the REST API and the frontend development environment in docker containers. Both of the servers are running in a live-reload mode so that when we make changes, they automatically update. Also, I wrote a quick python script to scrape Wikimedia links to the portraits of the politicians that we were displaying on our site. This way, the images will be up to date, and we save on storage.

---
#### What's in your way?
Nothing is blocking overall progress.

---
#### What will you do next week?
This next week we will wrap up Phase 2 and ensure that we get our website working in production mode. We need to make sure the website can connect to the REST API in production. Also, I need to help beautify some parts of the website.

---
#### If you read it, what did you think of The Liskov Substitution Principle?
The "Liskov Substitution Principle" is a good read. The article highlighted several design issues I encountered in the wild during my internship this past summer. I used RTTI in C++ to solve the problem, but now I see a better solution based on the examples in the article.

---
#### What was your experience with Test #1? (this question will vary, week to week)

I found Test #1 to be fun. It touched upon a lot of the concepts that we had covered during class and helped me gauge how much I've improved.

---
#### What made you happy this week?
The League of Legends World Championship is happening in China for the past couple of weeks. One of the teams I follow (G2 for those who know) had made it out of the group stage and today also made it to the semifinals.

---
#### What's your pick-of-the-week or tip-of-the-week?
Docker-compose is a useful tool for spinning up development environments locally that depend on multiple services. For our project, we have two main services: the REST API and the Front End development server. The first step is to create docker images that start these services in development mode or a live-reload mode. Then define a docker-compose.yml file where you describe the services that you need and how they should startup. For example, you may want to expose a particular port or mount a directory from the host machine. Once the file is defined, starting local development is as simple as running "docker-compose up."



<img src="/assets/headshot.jpg">
