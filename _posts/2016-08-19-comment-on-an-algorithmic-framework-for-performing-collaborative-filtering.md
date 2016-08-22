---
layout: post
title: "Comment on 'An Algorithmic Framework for Performing Collaborative
  Filtering'"
date: 2016-08-18 16:45:01 -0300
categories: recommendation-systems
---
(This comment is for Recommendation Systems course at PUC Chile)

In this work, the _Herlocker et al._ compare different
algorithm variants used in performing Collaborative Filtering. The following
prediction algorithm components where tested:

- Similarity Weight
- Significance Weighting
- Variance Weighting
- Selecting Neighborhoods
- Rating Normalization

I only have two minor comments for this work. My first observation is where the
authors introduce the Spearman rank correlation coefficient. They show the
following equation:

$$w_{a, u} = \frac{\sum_{i=1}^m (rank_{a,i} - \bar{rank}_a) \cdot
  (rank_{u, i} - \bar{rank}_u)}{\sigma_a \cdot \sigma_u}$$

but what does $$rank_{a, i}$$ mean? or how do I calculate $$\bar{rank}_a$$? The
authors don't explain this.

My other comment, is regarding the significance weighting section. The authors
say that $$50$$ commonly rated items, they applied a significance weighting of
$$\frac{n}{50}$$, where $$n$$ is the number of co-rated items. But they didn't
say how they selected that number. It was arbitrary or it was selected by
running experiments? If it was the later, it would have been interesting to
see how the accuracy changed when choosing a different threshold for the
commonly rated items.
