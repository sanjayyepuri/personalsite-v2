---
layout: post
title: "CS373 Fall 2020: Sanjay Yepuri"
description: "Introductory Post for CS373"
category:
tags: []
---
<img src="/assets/headshot.jpg">

Hi, I am Sanjay, a senior studying Computer Science and Math at UT Austin. Over the next couple of weeks, I will be writing a series of blog posts over various software engineering topics. But, first a little about myself.

> What high school did you attend? <br>
> What was your favorite extracurricular activity in high school?

I attended Seven Lakes High School in Katy, TX. My favorite extracurricular was UIL Computer Science. It was while I was on this team that I built my first web application and distributed system to judge Java programs. It was designed to handle over 400 competitors and employed various technologies such as Node, Angular, and RabbitMQ.

> Why are you in this class?

For the first time, I am leading a team of 8 people to build a web application for a non-profit that I helped start last April. The initial web app we built cut many corners. It had no testing, and the code quality was low. Now that we are growing (we have over 7000 active users) and other parts of our organization want features on the site, we decided to do a complete rewrite as opposed to refactoring the existing code.

I am taking this class to learn more about software engineering to build more maintainable and extendable software; hopefully, to even apply the knowledge to my current project.

> What's your pick-of-the-week or tip-of-the-week?

This week, I experimented with different ways of deploying a REST API in GCP. After evaluating Cloud Run and Cloud Functions, I decided to use Cloud Functions. Cloud Functions are very similar to AWS Lambda functions and are used to build serverless backends. I found it simple to convert my ExpressJS REST API server to run as a Cloud Function. I only had to change one line. The main drawback of this approach is that if my site doesn't receive a lot of traffic, the function instance will be shut down; the next user of my web app will incur the cold-start latency. From my testing, this latency was around ~3 seconds (up from ~200ms).
