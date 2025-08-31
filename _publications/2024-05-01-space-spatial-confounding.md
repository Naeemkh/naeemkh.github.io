---
title: "SpaCE: The Spatial Confounding Environment"
collection: publications
category: manuscripts
permalink: /publication/2024-05-01-space-spatial-confounding
excerpt: 'We introduce SpaCE: The Spatial Confounding Environment, the first toolkit to provide realistic benchmark datasets and tools for systematically evaluating causal inference methods designed to alleviate spatial confounding. The toolkit includes training data, true counterfactuals, spatial graphs with coordinates, and realistic semi-synthetic outcomes generated using state-of-the-art machine learning ensembles.'
date: 2024-05-01
venue: 'International Conference on Learning Representations (ICLR)'
paperurl: 'https://proceedings.iclr.cc/paper_files/paper/2024/file/d2155b1f7eb42350d7bc3013eefe5480-Paper-Conference.pdf'
citation: 'Tec, M., Trisovic, A., Audirac, M., Woodward, S., Hu, J., Khoshnevis, N., & Dominici, F. (2024). SpaCE: The Spatial Confounding Environment. In International Conference on Learning Representations (ICLR 2024).'
---

## Abstract

Spatial confounding poses a significant challenge in scientific studies involving spatial data, where unobserved spatial variables can influence both treatment and outcome, possibly leading to spurious associations. To address this problem, we introduce SpaCE: The Spatial Confounding Environment, the first toolkit to provide realistic benchmark datasets and tools for systematically evaluating causal inference methods designed to alleviate spatial confounding. 

Each dataset includes training data, true counterfactuals, a spatial graph with coordinates, and smoothness and confounding scores characterizing the effect of a missing spatial confounder. It also includes realistic semi-synthetic outcomes and counterfactuals, generated using state-of-the-art machine learning ensembles, following best practices for causal inference benchmarks. The datasets cover real treatment and covariates from diverse domains, including climate, health and social sciences. 

SpaCE facilitates an automated end-to-end pipeline, simplifying data loading, experimental setup, and evaluating machine learning and causal inference models. The SpaCE project provides several dozens of datasets of diverse sizes and spatial complexity. It is publicly available as a Python package, encouraging community feedback and contributions.

## Key Features

- **Comprehensive Benchmarking**: First systematic toolkit for evaluating spatial confounding methods
- **Realistic Datasets**: Semi-synthetic outcomes generated using state-of-the-art ML ensembles
- **Multi-Domain Coverage**: Datasets spanning climate, health, and social sciences
- **Complete Pipeline**: End-to-end automated pipeline for data loading and model evaluation
- **True Counterfactuals**: Includes ground truth counterfactuals for rigorous evaluation
- **Spatial Complexity**: Datasets with varying sizes and spatial complexity levels

## Impact and Availability

SpaCE addresses a critical gap in causal inference evaluation by providing standardized benchmarks for spatial confounding scenarios. The toolkit is publicly available as a Python package, fostering reproducible research and community collaboration in the important area of spatial causal inference. This work enables researchers to rigorously compare and develop new methods for handling spatial confounding in observational studies.

## Software Availability

The SpaCE toolkit is available as a Python package and encourages community feedback and contributions. This represents a significant contribution to the causal inference and spatial statistics communities by providing standardized evaluation tools for an important and challenging problem.
