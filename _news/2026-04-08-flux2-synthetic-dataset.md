---
date: 2026-04-08
title: "Released FLUX.2-dev Synthetic 2M — a large-scale text-to-image dataset on Hugging Face"
---

We released **FLUX.2-dev Synthetic 2M**, a large-scale synthetic text-to-image dataset, on Hugging Face, with a citable DOI: [10.57967/hf/8311](https://doi.org/10.57967/hf/8311).

The dataset contains roughly **2.28 million image–caption pairs** generated with the **FLUX.2-dev** diffusion model. It is intended to support research on text-to-image generation, synthetic data, and generative models.

**At a glance:**

- ~2,282,665 synthetic image–caption pairs
- Images generated with FLUX.2-dev at 512×512 resolution (50 inference steps, guidance scale 3.5)
- Captions sourced unmodified from the Text2Image-2M dataset
- Packaged as WebDataset — 571 shards (~4,000 samples each); each sample is a `.png` image, a `.txt` caption, and a `.json` metadata file recording the seed and generation parameters
- Generated through a distributed multi-GPU pipeline on the Kempner AI cluster

## A few samples

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px; margin: 30px 0;">
  <figure style="margin: 0;">
    <img src="/images/news/flux2-synthetic-2026/sample-01.png" alt="A woman in a hat stands in front of a colorful umbrella." style="width: 100%; height: auto; border-radius: 8px;" />
    <figcaption style="font-size: 0.85em; color: #555; margin-top: 8px;">&ldquo;A woman in a hat stands in front of a colorful umbrella.&rdquo;</figcaption>
  </figure>
  <figure style="margin: 0;">
    <img src="/images/news/flux2-synthetic-2026/sample-02.png" alt="A plate of Chinese food with dumplings, noodles, and vegetables." style="width: 100%; height: auto; border-radius: 8px;" />
    <figcaption style="font-size: 0.85em; color: #555; margin-top: 8px;">&ldquo;A plate of Chinese food with a variety of dishes including dumplings, noodles, and vegetables&hellip;&rdquo;</figcaption>
  </figure>
  <figure style="margin: 0;">
    <img src="/images/news/flux2-synthetic-2026/sample-03.png" alt="An open air sculpture with trees in the background." style="width: 100%; height: auto; border-radius: 8px;" />
    <figcaption style="font-size: 0.85em; color: #555; margin-top: 8px;">&ldquo;an open air sculpture with trees in the background&rdquo;</figcaption>
  </figure>
  <figure style="margin: 0;">
    <img src="/images/news/flux2-synthetic-2026/sample-04.png" alt="An animated young girl with green eyes and black hair eating noodles at an outdoor table." style="width: 100%; height: auto; border-radius: 8px;" />
    <figcaption style="font-size: 0.85em; color: #555; margin-top: 8px;">&ldquo;An animated figure, likely a young girl with green eyes and black hair, enjoys a meal of noodles at an outdoor wooden table&hellip;&rdquo;</figcaption>
  </figure>
</div>

The dataset is released for research use and is subject to the upstream FLUX.2-dev and Text2Image-2M licenses.

**Authors:** Naeem Khoshnevis, Gabriel Guo, Eric Vanden-Eijnden, Nicholas Boffi, and Michael S. Albergo (Kempner Institute, Harvard University).

- **Dataset:** [huggingface.co/datasets/KempnerInstituteAI/flux.2-dev-synthetic-2M](https://huggingface.co/datasets/KempnerInstituteAI/flux.2-dev-synthetic-2M)
- **DOI:** [10.57967/hf/8311](https://doi.org/10.57967/hf/8311)
