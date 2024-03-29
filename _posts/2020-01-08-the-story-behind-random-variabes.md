---
layout: post
title: More on Random Variables
description: “Random Variables are Random”
image: “”

category: 
tags: []
---

A *random variable* is a value which we do not know yet or we are uncertain of. They are the fundamental unit of statistics and are used anytime we want to predict a value. Having a good understanding of their properties makes it easier to model situations with statistics. In general, we know the values that a random variable could take on, and for each value, the probability of that value occurring. 

Let’s take the canonical example: a die roll. We will use a random variable $$D$$ to represent the value after a single roll of a fair die. It's important to understand that all random variables have a story or context behind them. In this scenario, when we roll a dice, there are 6 possible values (1, 2, ..., 6), each equally likely of occurring (a probability of 1/6).

This is how random variables are usually explained. However, more recently, I learned some more definitions that I found simple and easy to understand. 

The first being $$B$$-valued random variables. 

> Given a set $$B$$, we say that the random variable $$X$$ is $$B$$-valued if $$P[x \in B] = 1$$. 

In other words, the probability that a $$B$$-valued random variable takes on a value that is in the set $$B$$ is 1. Using our example above, the random variable, $$D$$, representing a die roll is $$\{1, 2, 3, ..., 6\}$$-valued. It also follows that the $$D$$ is also $$\{1, 2, ..., 6, 7\}$$-valued; the set $$B$$ does not necessarily need to be the smallest set that contains the values of the random variable. Essentially, as long as $$B$$ contains the values $$1...6$$, then $$D$$ is $$B$$-valued. Therefore, we can say $$D$$ is also $$\mathbb{N}$$ and $$\mathbb{R}$$-valued. 

Just knowing a set $$B$$ is usually not sufficient to describe a random variable since it may contain many values that our random variable will never take. The next definition will help. 

> The support $$\mathcal{S}_X$$ of the discrete random variable $$X$$ is the smallest set such that $$X$$ is $$\mathcal{S}_X$$-valued. 

So, while our random variable $$D$$ might be $$\mathbb{N}$$-valued, its support $$\mathcal{S}_D$$ is $$\{1, 2, ..., 6\}$$. This is the smallest set $$B$$ such that $$P[x \in B]$$ is 1; in otherwords, if we were to remove any value from $$\mathcal{S}_D$$ and form $$B$$, then the $$P[x \in B] < 1$$.

Now we can use these two concepts to discuss other concepts we already know. For example, we may use these definitions to formalize the definition of discrete random variables. Or maybe characterize types of random variables such as Bernoulli random variables.
