---
layout: archive
permalink: /projects/
author_profile: true
---

{% include base_path %}

The following are some current active areas of research.

## Semi-parametric statistics in inconsistency regimes

<img align="left" src='/images/debiasing.jpg' width='500px' height='315px' style="padding: 0px 20px 10px 0px;">

Increasingly in science,
researchers have access to complex, high-dimensional data,
from rich sequencing data in biology to various imaging modalities in medicine to detailed demographic and socioeconomic information in economics.
Machine learning models have dramatically enhanced our ability to make accurate predictions on the basis these complex covariates.
Often, however, the end goal is not a prediction, but rather estimation and uncertainty quantification for a few scientifically meaningful parameters like a causal effect or a conditional association.
The mathematical framework for understanding how to leverage predictions for inference on target parameters is semi-parametric statistics.
In this framework, we call the parameters of interest, such as causal effects, ''target parameters,'' and the high-dimensional or non-parametric parameters describing the prediction models ''nuisance parameters.''

Typically, this literature focuses on cases where some of the nuisance parameters can be estimated extremely well, sometimes so well that errors in nuisance estimation negligibly degrade estimation of the target parameter.
In practice, it may not be safe to assume that nuisance parameter estimates are this accurate.

I am currently leveraging ''exact asymptotics'' to develop semi-parametric methods and guarantees in settings where high-dimensional parameters cannot be estimated consistently. ''Exact asymptotics'' refers to a set of mathematical tools for deriving precise characterizations of the errors made by complex, high-dimensional statistical methods, especially in cases where there errors are not small. My work has led to novel algorithms for estimation and inference of [conditional correlations](https://arxiv.org/abs/2107.14172) and [population means with missing data](https://arxiv.org/abs/2309.01362) with high-dimensional nuisance parameters.

The long-term goal is to find practical methods to mitigate bias and quantify uncertainty resulting from errors in complex predictions models, improving estimation and enabling valid inference.

Representative papers can be found [here](https://arxiv.org/abs/2007.13716) and especially [here](https://arxiv.org/abs/2107.14172) and [here](https://arxiv.org/abs/2309.01362).

## High-dimensional variational Bayes
 
Computationally, Markov Chain Monte Carlo (MCMC) methods for performing inference in high-dimensional statistical models can be prohibitively expensive.
Variational methods are an approximate approach to Bayesian inference which can be substantially more efficient.
Unlike MCMC methods, which are based on sampling, variational method are based on optimization.

Variational methods approximate posterior distributions by a simpler class of distributions. A popular choice is is the ''mean-field approximation,'' in which subsets of variables are approximated as independent. It has been observed both empirically and theoretically that the mean-field approximation often leads to underestimates of posterior uncertainty, which can lead to excessively short credible intervals and inflated error rates in variable selection.

In certain high-dimensional settings, including generalized linear regression, Bayesian PCA, and community detection, corrections to naive mean field approaches based on the TAP free energy from statistical physics have been proposed. I am interested in rigorously analyzing these approaches, and in particular, establishing that they provide an efficient approach to computing consistent approximations of posterior marginals.

Perhaps interestingly, this line of work has some relationship to the ''semi-parametric statistics in inconsistency regimes'' direction described above. Appropriately viewed, naive mean field's underestimation of posterior uncertainty results from insufficient accounting of the impact of errors in certain ''nuisance parameters.''

Although variational inference is typically viewed as an alternative to sampling, recently there has been interest in its use as as sub-routine of sampling algorithm. A novel sampling approach called ''stochastic localization'' has recently been proposed which is able to sample from complex, high-dimensional probability distributions given access to a sub-routine which computes moments of that (and related) distributions. This approach is related to diffusion models.
Variational methods may be used to compute these moments. My work on the TAP free energy for $\mathbb{Z}_2$-synchronization established the viability of this approach for sampling from the Sherrington-Kirkpatrick Gibbs measure, a quintessential model of a random, non-convex optimization problem studied extensively in physics and computer science. This resolved a conjecture of Alaoui, Selkke, and Montanari and established the possibility of sampling from this distribution efficiently throughout the regime in which it had been widely conjecture to be possible.
 
## Dynamics and optimality of first order methods

## Fitness inference in phylogenetics








