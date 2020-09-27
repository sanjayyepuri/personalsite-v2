---
layout: post
title: "CS373 Fall 2020 Week 5 - Sanjay Yepuri"
description: "Week of 21 Sept. - 27 Sept."
category:
tags: []
---

#### What did you do this past week?

This past week, I mainly focused on school work. For Coved, I reimplemented a sign-in page to make setup the form validation libraries and also make the component responsive. Our team for the IDB1 project had settled on a project to help US voters be informed about ongoing elections. As Election Day nears, hopefully, this project can be useful to get a better idea where various candidates stand on issues and what they have been saying on social media. .

---
#### What’s in your way?

There isn’t much that is blocking progress.

---
#### What will you do next week?

This following week our team and I will start building out our static website and designing the customer-facing API. For the website, we are planning on using bootstrap. This should make it easy to make sure everything is responsive. In addition to this, we will work on setting CI/CD and our testing framework. Once these tasks are completed, we will start work on the first technical report. .

---
#### What was your experience of *types*, *object models*, and *iterators*? (this question will vary, week to week)

My experience with types in python has been interesting. For a previous internship, I had bind some c++ code and extend C++ classes. Since C++ is statically typed, it was important to ensure that the python types are correct.

---
#### How are you doing and holding up? What’s been most helpful for you in terms of support at this time?

I moved to Austin, so it has been cool to see my friends again.

---
#### What made you happy this week?
There hasn't been anything this week to make me not happy.

---
#### What’s your **pick-of-the-week** or **tip-of-the-week**?

My pick of the week is Docker’s multi-stage build. This also allows for various stages of the build to occur in separate temporary containers and then share artifacts between each stage. This ensures that the final docker image contains only the files and dependencies it needs keeping the final image size small. In our project, we are using a multi-stage build for building our front end docker image. This docker image is responsible for hosting the static assets and running a web server. Our first stage builds the React project; the final stage then copies the build artifacts (the static assets) and stores them in the directory that nginx will serve on port 80.

<img src="/assets/headshot.jpg">
