---
layout: post
title: "Comment on 'Context-aware recommender systems'"
date: 2016-09-18 16:45:01 -0300
categories: recommendation-systems
---
(This comment is for Recommendation Systems course at PUC Chile)

In this paper, the Adomavicius and Tuzhilin discuss recommender systems that
use the user context to make recommendations.

The book chapter discusses three ways to include context information in the
system: pre-filtering, post-filtering and contextual modeling. The decision
on which of this we should use when designing a CAS depends on the particular
domain where we are going to apply our recommendation system. I found
interesting the hierarchical regression-based Bayesian preference model for
contextual modeling. Usually, by using bayesian models we can have a coherent
treatment of uncertainty, and sometimes this is very useful. But, it have
the disadvantage that it can be slow.

One thing that the authors didn't discuss in this book chapter is the 
several privacy considerations we need to take care when developing a
context-aware system. Securing user privacy is very important nowadays, and we
as a user expect that any CAS use strict privacy policies to protect our data.
Also, CAS need to be careful when the user doesn't want to share some
contextual data such as their location. Having this things in consideration
when designing the context-aware system helps a lot to improve user 
trust in it.
