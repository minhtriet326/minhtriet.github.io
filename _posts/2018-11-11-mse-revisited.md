---
layout: post
comments: true
mathjax: true
---

MSE page in Wikipedia states the relation between Bias and Variance, namely $$MSE(\hat\theta)=Variance(\hat\theta) + Bias^2(\hat\theta, \theta)$$, in which $$\hat\theta$$ is the prediction and $$\theta$$ is the correct value.

Since $$Variance$$ and $$Bias^2$$ both non-negative, it would follow that a perfect estimator would have zero variance and zero bias. Zero variance should mean the output of the estimator is always equal to its expected values. Zero bias means $$E(\hat\theta)) - \theta = 0$$. That enforces that \theta must be a contant. If we consider the common cases of predicting $$Y$$ using $$X$$, this equation would look like forcing $$Y$$ to be the same, since we only have one $$E(\hat\theta)$$.

If you have spotted the wrongness in the reasoning, congrats.

The key here is to remember that this is not just any estimator, but a parameter estimator. If you use the mindset of a mapping function from $$X$$ to $$Y$$, confusion may happen. In this case, $$\hat\theta$$ should not be confused with $$X$$
