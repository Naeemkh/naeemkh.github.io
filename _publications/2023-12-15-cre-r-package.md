---
title: "CRE: An R package for interpretable discovery and inference of heterogeneous treatment effects"
collection: publications
category: manuscripts
permalink: /publication/2023-12-15-cre-r-package
excerpt: 'CRE is an R package providing a flexible implementation of Causal Rule Ensemble, a new method for interpretable heterogeneous treatment effect (HTE) characterization in terms of decision rules, via an extensive exploration of heterogeneity patterns by an ensemble-of-trees approach. The package addresses limitations of single-tree heterogeneity discovery including instability and reduced exploration of potential heterogeneity.'
date: 2023-12-15
venue: 'Journal of Open Source Software'
paperurl: 'https://joss.theoj.org/papers/10.21105/joss.05587.pdf'
citation: 'Cadei, R., Khoshnevis, N., Lee, K., Garcia, D. M., & Bargagli-Stoffi, F. J. (2023). CRE: An R package for interpretable discovery and inference of heterogeneous treatment effects. Journal of Open Source Software, 8(92), 5587. https://doi.org/10.21105/joss.05587'
---

## Abstract

In health and social sciences, it is critically important to identify interpretable subgroups of the study population where a treatment has notable heterogeneity in the causal effects with respect to the average treatment effect (ATE). Several approaches have already been proposed for heterogeneous treatment effect (HTE) discovery, either estimating first the conditional average treatment effect (CATE) and identifying heterogeneous subgroups in a second stage (Bargagli-Stoffi et al., 2020, 2022; Foster et al., 2011; Hahn et al., 2020), either estimating directly these subgroups in a direct data-driven procedure (Nagpal et al., 2020; Wang & Rudin, 2022). 

Many of these methodologies are decision tree-based methodologies. Tree-based approaches are based on efficient and easily implementable recursive mathematical programming (eg, HTE maximization), they can be easily tweaked and adapted to different scenarios depending on the research question of interest, and they guarantee a high degree of interpretability—ie, the degree to which a human can understand the cause of a decision (Lakkaraju et al., 2016). Despite these appealing features, single-tree heterogeneity discovery is characterized by two main limitations: instability in the identification of the subgroups and reduced exploration of the potential heterogeneity. 

To accommodate these shortcomings, Bargagli-Stoffi et al. (2023) proposed Causal Rule Ensemble, a new method for interpretable HTE characterization in terms of decision rules, via an extensive exploration of heterogeneity patterns by an ensemble-of-trees approach. CRE is an R package providing a flexible implementation of this methodology.

## Key Features

- **Interpretable HTE Discovery**: Identifies subgroups with heterogeneous treatment effects using decision rules
- **Ensemble Approach**: Overcomes limitations of single-tree methods through ensemble-of-trees methodology
- **Flexible Implementation**: Adaptable to different research scenarios and questions
- **Stability**: Addresses instability issues common in single-tree heterogeneity discovery
- **Comprehensive Exploration**: Enhanced exploration of potential heterogeneity patterns

## Software Availability

The CRE R package is available on CRAN and the source code is available on GitHub. This work contributes to the field of causal inference by providing researchers with interpretable tools for discovering heterogeneous treatment effects in observational and experimental data.
