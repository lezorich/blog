---
layout: post
title: "Comment on 'How Not To Sort By Average Rating'"
date: 2016-08-10 16:45:01 -0300
categories: recommendation-systems
---
(This comment is for Recommendation Systems course at PUC Chile)

I think that the author does a great job showing why simple solutions don't
work, and he proposes the lower bound of 
[Wilson score](https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval#Wilson_score_interval)
confidence interval for a Bernoulli parameter as the sorting score. Even though
the proposed score is better than, for example, taking the average rating as 
the score, it won't work in more complex scenarios. What if we want to take
into account the submission time of the content in the ranking? Or if we don't
only have positive/negative ratings but instead a number between 1 and 5 (like 
in the Amazon site)? The author doesn't mention this.

Also, I think that he misinterpret the meaning of a confidence interval. He
says that the question we want to answer is:

> Given the ratings I have, there is a 95% chance that the "real" fraction of 
positive ratings is at least what?

but a 95% confidence interval doesn't mean that there is a 95% probability 
that the "real" fraction of positive ratings lie within the calculated
interval. It means that there is a 95% of probability that <cite>calculated
confidence interval from some future experiment encompasses the true value
</cite> (from 
[Wikipedia](https://en.wikipedia.org/wiki/Confidence_interval#Meaning_and_interpretation)).
This is a probability about the confidence interval, not about the parameter.
