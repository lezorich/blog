---
layout: post
title: "Comment on 'Don't Look Stupid: Avoiding Pitfalls when Recommending
  Research Papers"
date: 2016-10-16 16:48:01 -0300
categories: recommendation-systems
---
(This comment is for Recommendation Systems course at PUC Chile)

I found this paper very interesting. In particular, I found interesting
the **Don't Look Stupid** principle, that says that we should only show
recommendations to users when we have some confidence in their usefulness. The
authors of the paper say that showing only one horrible recommendation is enough
for users to lose confidence in the recommender.

The paper also talks about the importance of selecting the right algorithm
for the specific domain we are targeting, and that we should evaluate 
that algorithm with real users. For example, the Naive Bayes algorithm performed
well in offline simulation experiments, scoring well on the accuracy metrics.
But, the experiments done with Naive Bayes with real users showed
that the users were not satisfied by the recommendation list returned
from this algorithm. This is very important, because it means that before
putting a recommendation system in production, we probably need to test it
with real users first and in my specific domain, so we **Don't Look Stupid** to
our users.  One option is to do A/B testing and evaluate several algorithms till we find
the best one.
