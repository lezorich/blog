---
layout: post
title: "Comment on 'Collaborative Filtering Recommender System' chapter"
date: 2016-08-10 16:45:01 -0300
categories: recommendation-systems
---
(This comment is for Recommendation Systems course at PUC Chile)

Collaborative Filtering Recommender System is a chapter of the The Adaptive
Web book by Schafer, Frankowski, Herlocker and Sen. It is basically a review
of the core concepts of Collaborative Filtering, with its primary uses and the
theory and practice of CF algorithms.

I think it is a great reading for someone that is not familiar with CF. It is
clear and well written. But, there are some things that where not very clear
to me. For example, in the User-Based Nearest Neighbour Algorithm, in eq (4)
the author says that we can compensate for ratings scale variation using the
user's mean ratings:

$$pred(u, i) = \bar{r}_u + \frac{\sum_{n \subset neighbours(u)}userSim(u, n)
\cdot (r_{ni} - \bar{r}_n)}{\sum_{n \subset neighbours(u)}userSim(u,n)}$$

but, it is not clear for the average rating term $$\bar{r}_n$$ is for all
user items, or only the corated ones.

Later in the same algorithm, the authors also say that we may choose not to
use negative correlations. The authors say that negative correlations are
generally believed to not be valuable in increasing prediction accuracy. I
know that a negative correlation means that the more I like something,
the more the other user dislike it. Intuitively, I was thinking that may be
this was a useful information to know in order to make a recommender system, but the
author didn't expanded on this. I was expecting a little more in depth analysis
of what is the benefit of using or discarding negative correlations.

Also, when the authors are talking about how clustering can help in reducing
the User-Based CF algorithm processing time, is not clear to me how it helps.
For example, he mentions k-means, but that algorithm usually needs several
passes through the data in order to build the clusters. In class we saw that
we generally do an offline preprocessing where we build the clusters, and then
we use those clusters to do the recommendation, but the text doesn't mention
this.
