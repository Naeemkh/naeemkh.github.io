---
title: "GPCERF-An R package for implementing Gaussian processes for estimating causal exposure response curves"
collection: publications
category: manuscripts
permalink: /publication/2024-03-13-gpcerf-r-package
excerpt: 'We present the GPCERF R package, which employs a novel Bayesian approach based on Gaussian Process (GP) to estimate the causal exposure-response function (CERF) for continuous exposures, along with associated uncertainties. The package provides a two-step end-to-end solution for causal inference with continuous exposures equipped with automatic and efficient uncertainty quantification.'
date: 2024-03-13
venue: 'Journal of Open Source Software'
paperurl: 'https://joss.theoj.org/papers/10.21105/joss.05465.pdf'
citation: 'Khoshnevis, N., Ren, B., & Braun, D. (2024). GPCERF-An R package for implementing Gaussian processes for estimating causal exposure response curves. Journal of Open Source Software, 9(95), 5465. https://doi.org/10.21105/joss.05465'
---

## Abstract

We present the GPCERF R package, which employs a novel Bayesian approach based on Gaussian Process (GP) to estimate the causal exposure-response function (CERF) for continuous exposures, along with associated uncertainties. R packages that target causal effects under a binary exposure setting exist (eg, Ho et al., 2011), as well as in the continuous exposure setting (eg, Khoshnevis et al., 2023). However, they often rely on a separate resampling stage to quantify uncertainty of the estimates. GPCERF provides a two-step end-to-end solution for causal inference with continuous exposures that is equipped with automatic and efficient uncertainty quantification. 

During the first step (the design phase), the algorithm searches for optimal hyperparameters (using the exposures and covariates) that achieve optimal covariate balance in the induced pseudo-population, ie, that the correlation between the exposure and each covariate is close to zero. The selected hyperparameters are then used in the second step (the analysis phase) to estimate the CERF on the balanced data set and its associated uncertainty using two different types of GPs: a standard GP and a nearest-neighbor GP (nnGP). The standard GP offers high accuracy in estimating CERF but is also computationally intensive. The nnGP is a computationally efficient approximation of the standard GP and is well-suited for the analysis of large-scale datasets.

## Software Availability

The GPCERF R package is available on CRAN and the source code is available on GitHub. This work contributes to the growing field of causal inference for continuous treatments by providing researchers with an accessible and efficient tool for estimating causal exposure-response relationships.
