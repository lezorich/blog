---
layout: post
title: "Comment on 'Slope One Predictors for Online Rating-Based Collaborative
  Filtering'"
date: 2016-08-20 16:45:01 -0300
categories: recommendation-systems
---
(This comment is for Recommendation Systems course at PUC Chile)

In this paper, _Lemire and Maclachlan_ propose three predictors of the form
$$f(x) = x + b$$, that work by precomputing the average difference between
the ratings of a pair of items for users who rated both. The main contribution
of their proposal is that they are competitive with memory-based algorithms
(like the popular Pearson correlation based algorithm), while being more
scalable and efficient.

The paper is very short, but I think that they explain their algorithm very
well, except for their set cardinality notation (they used $$card(\cdot)$$ 
instead of using the more readable $$\mid \cdot \mid$$). I also find very 
interesting the idea behind this algorithm, which is basically using the
difference of the ratings between a pair of items, and then adjust the slope 
one predictor.

My big comment about this paper is that, in my opinion, you can't say that
your algorithm is more efficient without actually showing the running time of
your method versus the others. The authors only compared the Mean Average
Error, and nothing else.  It also could have been very interesting to see a 
table with the memory usage of the different algorithms.
