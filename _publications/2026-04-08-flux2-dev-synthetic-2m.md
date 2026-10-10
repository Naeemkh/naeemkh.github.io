---
title: "FLUX.2-dev Synthetic 2M: a large-scale synthetic text-to-image dataset"
collection: publications
category: datasets
permalink: /publication/2026-04-08-flux2-dev-synthetic-2m
excerpt: 'A citable Hugging Face dataset of about 2.28 million image-caption pairs generated with the FLUX.2-dev diffusion model on the Kempner AI cluster, packaged as 571 WebDataset shards with per-sample generation metadata.'
date: 2026-04-08
venue: 'Hugging Face Datasets, KempnerInstituteAI (DOI 10.57967/hf/8311)'
paperurl: 'https://huggingface.co/datasets/KempnerInstituteAI/flux.2-dev-synthetic-2M'
citation: 'Khoshnevis, N., Guo, G., Vanden-Eijnden, E., Boffi, N., & Albergo, M. S. (2026). FLUX.2-dev Synthetic 2M [Data set]. Hugging Face. https://doi.org/10.57967/hf/8311'
---

## About the dataset

FLUX.2-dev Synthetic 2M is a large-scale synthetic text-to-image dataset released on Hugging Face with a citable DOI, [10.57967/hf/8311](https://doi.org/10.57967/hf/8311). It is intended to support research on text-to-image generation, synthetic data, and generative models.

- About 2,282,665 synthetic image-caption pairs
- Images generated with FLUX.2-dev at 512x512 resolution (50 inference steps, guidance scale 3.5)
- Captions sourced unmodified from the Text2Image-2M dataset
- Packaged as WebDataset, 571 shards of about 4,000 samples each; every sample is a `.png` image, a `.txt` caption, and a `.json` metadata file recording the seed and generation parameters
- Generated through a distributed multi-GPU pipeline on the Kempner AI cluster

The dataset is released for research use and is subject to the upstream FLUX.2-dev and Text2Image-2M licenses. See the [release note](/news/2026-04-08-flux2-synthetic-dataset/) for samples.
