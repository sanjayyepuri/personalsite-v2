---
layout: post
title: "CS373 Fall 2020 Week 7 - Sanjay Yepuri"
description: "Week of 5 Oct. - 11 Oct."
category:
tags: []
---
#### What did you do this past week?
This past week I found myself in a lul of classwork; I decided to take a breather and slow myself down. I did a little bit of research about styling websites and React-Bootstrap. I always found styling a react app to be a little bit more nuanced than styling an ordinary static web site.

---
#### What's in your way?
Currently, I have nothing blocking progress. I am waiting on certain API endpoints and models to be finalized before I  decide what gets displayed on the various detail pages on the website. However, while the work on the backend is being done, I can start designing the overall website.

---
#### What will you do next week?
This coming week, I will help set up the development infrastructure for the backend; this entails creating a docker image that can be used for both local development and testing in the build environment on Gitlab. In addition to this, I will help my teammates get up to speed on Flask and help them build some simple API endpoints.

---
#### If you read it, what did you think of The Open-Closed Principle?
This article is a really nice formalization of the "rules" of object-oriented design. We want to close modules/classes to change and open them to be extended. The Shape example that made it really to understand. In particular, when the author closes the DrawFunction to shape ordering was interesting. The first approach with creating a Precedes function that was to be overridden by child classes of Shape would be the way I would have tried to solve the problem. The "data-driven" approach the author showed was something I may try to look into more.

---
#### What was your experience of iterators, generators, and yield? (this question will vary, week to week)

Iterators and generators are very useful abstractions provided by Python. From my experience, python for-loops are slow for accessing elements. Iterators and other operations such as map or filter give a huge runtime speed over traditional loops.

---
#### What made you happy this week?
I had a small break between large projects.

---
#### What's your pick-of-the-week or tip-of-the-week?
My pick of the week is functional components in React and React Hooks. This is a method of defining a component using a single function rather than defining a class and extending React-Component. From my experience, this leads to less code that is simpler. Functional components don't have the various lifetime methods that you can override; rather, components can be updated using React Hooks.



<img src="/assets/headshot.jpg">
