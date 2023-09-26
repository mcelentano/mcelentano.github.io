---
layout: archive
permalink: /projects/
author_profile: true
---

{% include base_path %}

The following are some of my current active areas of research.

## Semi-parametric statistics in inconsistency regimes

<img align="left" src='/images/debiasing.jpg' width='500px' height='315px' style="padding: 0px 20px 10px 0px;">

Increasingly in science,
researchers have access to complex, high-dimensional data,
from rich sequencing data in biology to various imaging modalities in medicine to detailed demographic and socioeconomic information in economics.
Machine learning models have dramatically enhanced our ability to make accurate predictions on the basis these complex covariates.
Often, however, the end goal is not a prediction, but rather estimation and uncertainty quantification for a few scientifically meaningful parameters like a causal effect or a conditional association.
The mathematical framework for understanding how to leverage predictions for inference on target parameters is semi-parametric statistics.
In this framework, we call the parameters of interest, such as causal effects, ''target parameters,'' and the high-dimensional parameters describing the prediction models ''nuisance parameters.''

Typically, this literature focuses on cases where some of the nuisance parameters can be estimated extremely well, sometimes so well that errors in nuisance estimation negligibly degrade estimation of the target parameter.
In practice, it may not be safe to assume that nuisance parameter estimates are this accurate.

I am currently leveraging ''exact asymptotics'' to develop semi-parametric methods and guarantees in settings where high-dimensional parameters cannot be estimated consistently. ``Exact asymptotics'' refers to a set of mathematical tools for deriving precise characterizations of the errors made by complex, high-dimensional statistical methods, especially in cases where there errors are not small. My work has led to novel algorithms for estimation and inference of [conditional correlations](https://arxiv.org/abs/2107.14172) and [population means with missing data](https://arxiv.org/abs/2309.01362) with high-dimensional nuisance parameters.

The long term goal is to find corrections to existing methods which mitigate bias resulting from errors in complex predictions models, improving estimation and enabling valid inference.

Representative papers: [here](https://arxiv.org/abs/2007.13716), [here](https://arxiv.org/abs/2107.14172), and [here](https://arxiv.org/abs/2309.01362).

## Dynamics and optimality of first order methods

## Variational Bayesian inference

## Fitness inference in phylogenetics