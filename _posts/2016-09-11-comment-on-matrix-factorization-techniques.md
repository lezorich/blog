---
layout: post
title: "Comment on 'Matrix factorization techniques for recommender systems'"
date: 2016-09-11 16:48:01 -0300
categories: recommendation-systems
---
(This comment is for Recommendation Systems course at PUC Chile)

This paper was published in 2009, and it explains what is matrix factorization
and how we can use it to recommend items.

I think the paper is very clear, it explains most of the parameters of the 
equations, and it also gives all the intuitions of the different techniques
used. I also liked that the paper addressed the cold start problem, and it
proposes adding additional sources of information about the users if they 
have supplied very few ratings.

In the paper the authors also explain the model they used to compete in the
Netflix prize, showing the RMSE they got with different models and different
parameters.

I was expecting the authors to show the time and memory of matrix factorization
versus the other models. In several sections of the paper the authors claim
that matrix factorization is more efficient, but they didn't showed any 
evidence regarding this.
