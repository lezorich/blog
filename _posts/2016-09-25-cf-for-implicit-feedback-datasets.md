---
layout: post
title: "Comment on 'Collaborative Filtering for Implicit Feedback Datasets'"
date: 2016-09-25 16:45:01 -0300
categories: recommendation-systems
---
(This comment is for Recommendation Systems course at PUC Chile)

This paper by Hu _et al_, the authors explain the challenges we face when 
using implicit feedback for recommendations, and also they propose a factor
model that uses implicit feedback for making the recommendations.

In general I think that the paper is very clear. I really liked that they
analized the complexity of the algorithm, something that I haven't seen in
previous papers I read for this course. After this analysis, the authors
suggests a scalable optimization procedure that scales linearly with the
size of the input.

I also liked that they introduced this confidence level $$c_{ui}$$ that measures
the confidence we have of the user $$u$$ consuming item $$i$$. This is useful
because the user may watch a TV show just because he stayed on the channel
of the previously watched show. This variable let's us measure the confidence
that the user liked that show.

Lastly, I also really liked that they provide a way to compute the explanations
of why the method recommended what it recommended. This is very important
because it helps to improve the users trust in the recommending system.

As a negative aspect, I think it would be interesting to show the execution
time and the memory that the proposed algorithm used in the experiments run.
I know they made a complexity analysis of the algorithm, and that the paper
is a few years old, but nowadays when we have lots of data is very important
to know the efficiency of the different algorithms.
