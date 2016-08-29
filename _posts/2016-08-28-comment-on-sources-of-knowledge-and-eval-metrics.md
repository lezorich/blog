---
layout: post
title: "Comment about 'Recommender Systems: Sources of Knowledge and Evaluation
  Metrics'"
date: 2016-08-28 15:45:01 -0300
categories: recommendation-systems
---
(This comment is for Recommendation Systems course at PUC Chile)


*Sources of Knowledge and Evaluation Metrics* is a book chapter that present
a classification of recommender systems and then the author focus on presenting
the sources of knowledge and evaluation metrics for this type of systems.

I think that first part of the chapter explains very well the different types
of recommender systems, giving some example algorithms with their strengths
and weaknesses.

In the sources of knowledge section, the authors talked about context data as
input for recommendation systems. In particular, they mention that now, with the proliferation
of mobile devices, recommendation systems can now use the user location
information to make better recommendations. But the authors didn't mention the
precautions we need to have before using the user location data. For example,
some users may prefer **not** to share their location with the system, so
usually before tracking the user location, we need to explicitly ask the user
if they accept it or not in order to respect their privacy.

Lastly, in the evaluation metrics I found most metrics very clear to
understand, except **Intra-list Similiarity**. When talking about Intra-list
Similarity metric, defined as

$$
ILS(P_{w_i}) = \frac{\sum_{b_k \in P_{w_i}}\sum_{b_k \in P_{w_i}, b_k \neq b_c}c_0(b_k, b_c)}{2}
$$

the authors didn't explain anything. The intuition behind is that higher scores
of ILS denote lower diversity, but they didn't explain the meaning of any
term in the formula above.
