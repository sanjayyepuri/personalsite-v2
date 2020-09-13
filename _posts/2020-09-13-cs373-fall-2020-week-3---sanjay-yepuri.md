---
layout: post
title: "CS373 Fall 2020: Week 3 - Sai Yepuri"
description: "Week of 7 Sept. - 13 Sept."
category:
tags: []
---
#### What did you do this past week?

In this past week, I forked the repository on Gitlab and then cloned it locally on my machine. Then, I looked through the code and got familiar with the started code and the features that exist in Gitlab. I also updated Docker and tested running the codebase locally using  Downing’s docker image.

Once I was familiar with the codebase, I fixed the test cases and implemented the simplest solution to Collatz. I thought of some edge cases that could appear and added corresponding unit tests. Once I had a working implementation, I started to add the optimizations. As I was working, I  continued to think of edge cases and added unit tests.

---
#### What’s in your way?

Nothing.

---
#### What will you do next week?

Next week, I am planning to get some outstanding tasks done for coved.org. We are getting close to launching version 2, but a lot of work needs to be done. Also, I am going to take a look at Julia and possibly use it to build a project. From what I have read, it seems like a cool alternative to the likes of Python and Swift.

---
#### What was your experience of **Collatz**, **the starter code**, **the makefile**, its **optimizations**, and **exceptions**?

I felt that the codebase was fine. I modified the makefile so that the stopped container will remove itself once I exit the shell..

---
#### How are you doing and holding up? What’s been most helpful for you in terms of support at this time?

I am doing great. Piazza and classmates have helped me stay on track and answer any questions I had about the project.

---
#### What made you happy this week?

One of my biggest gripes with large projects in Python is the lack of type information. To use a function, I would either read the documentation or read through the code to figure an arguments’ type. The MyPy library is a great addition to add type annotations and checking.

---
#### What’s your **pick-of-the-week** or **tip-of-the-week**?

My pick-of-the-week is the `func_tools library`. Initially, I implemented caching by creating a map but then read about a decorator `lru_cache` that caches function calls. First, I made a recursive function to compute cycle lengths. Then, I was able to add the decorator and immediately get the benefits of caching. The reason for making the computation recursive was so that intermediate values were also cached. This optimization improved my cache hit rate by about 50%.
