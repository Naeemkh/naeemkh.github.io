---
date: 2026-06-09
title: Introduced KempnerForge at the 2026 Research Computing and Data Summit at Harvard
---

I had the opportunity to introduce **KempnerForge** at the [2026 Research Computing and Data Summit](https://rc.harvard.edu/2026/05/01/harvard-rcd-summit-2026/) at Harvard.

<div style="text-align: center; margin: 30px 0;">
  <img src="/images/news/rcd-summit-2026/IMG_0600.JPG" alt="Presenting KempnerForge at the 2026 RCD Summit, Harvard" style="max-width: 800px; width: 100%; height: auto; border-radius: 8px;" />
</div>

KempnerForge is an open-source, PyTorch-native training framework developed by the Research Engineering Team at the Kempner Institute. It is designed for reliable foundation-model training on shared AI clusters, where interruptions, preemptions, changing allocations, and heterogeneous research workloads are part of everyday life.

KempnerForge is built to make large-scale training more reliable, reproducible, and easier to operate on real shared infrastructure.

Key features include:

- Preemption-safe checkpointing and auto-resume
- Distributed checkpointing with N-to-M resharding
- SLURM-native multi-node launch
- FSDP2, tensor parallelism, expert parallelism, pipeline parallelism, and FP8 support
- Dense, MoE, and vision-language model support
- Typed TOML configuration validated before training starts
- NaN detection, NCCL/GPU health checks, and profiler integration
- MFU tracking, WandB/TensorBoard logging, and reproducible runs

If you are training foundation models on a shared AI cluster, KempnerForge is built for you.

---

- **Full Presentation:** [Download the slides (PDF)](/images/news/rcd-summit-2026/kempnerforge-rcd-summit-2026.pdf)
- **Project Repository:** [github.com/KempnerInstitute/KempnerForge](https://github.com/KempnerInstitute/KempnerForge)

---

## Photo Gallery

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 30px 0;">
  <img src="/images/news/rcd-summit-2026/IMG_7089.jpeg" alt="RCD Summit 2026 — Speaking" style="width: 100%; height: 250px; object-fit: cover; border-radius: 8px;" />
  <img src="/images/news/rcd-summit-2026/IMG_7642.JPEG" alt="RCD Summit 2026 — Audience view" style="width: 100%; height: 250px; object-fit: cover; border-radius: 8px;" />
  <img src="/images/news/rcd-summit-2026/IMG_7657.JPEG" alt="RCD Summit 2026 — Closing slide" style="width: 100%; height: 250px; object-fit: cover; border-radius: 8px;" />
  <img src="/images/news/rcd-summit-2026/IMG_7658.JPEG" alt="RCD Summit 2026 — Q&A" style="width: 100%; height: 250px; object-fit: cover; border-radius: 8px;" />
</div>
