---
date: 2026-03-16
title: Hosted Large Language Model Distributed Inference Workshop at Harvard
---

I recently hosted a hands-on workshop at Harvard University, focused on the technical challenges and solutions for Large Language Model (LLM) Distributed Inference. As both a Lead ML Research Engineer and a PyTorch Ambassador, my goal was to bridge the gap between theoretical AI models and the high-performance computing (HPC) infrastructure required to serve them at scale.

The workshop provided a deep dive into the LLM lifecycle, specifically focusing on the Deployment and Monitoring phase. We explored several key technical areas:

- **Inference Engines:** How vLLM functions within the AI ecosystem to solve bottlenecks like serial execution and static VRAM allocation.

- **PagedAttention:** A look at how vLLM’s core innovation eliminates memory waste by partitioning the KV cache into non-contiguous physical blocks.

- **Multi-GPU Scaling:** Strategies for sharding massive models, such as Llama 3 405B, using Tensor Parallelism (TP) and Pipeline Parallelism (PP) across multi-node clusters.

- **Continuous Batching:** Demonstrating how dynamic request injection and the removal of sync barriers significantly improve GPU occupancy and reduce latency.

During the hands-on labs, participants accessed the Kempner HPC cluster to run offline batch inference and deploy their own vLLM inference servers, interacting with model endpoints via OpenAI-compatible APIs and monitoring real-time activity with nvtop.

All materials, including the lab guides and code, are available in the public repository:

- **Workshop Materials:** [https://github.com/KempnerInstitute/distributed-inference-vllm](https://github.com/KempnerInstitute/distributed-inference-vllm/tree/main/workshops/w260326)

- **Full Presentation:** [LLM Distributed Inference Slides](https://docs.google.com/presentation/d/1dIwQRIJnrVy-WZr3-BfhWGCo_tZzZVB2/edit?usp=sharing&ouid=110906857987716901096&rtpof=true&sd=true)

---

## Special Thanks

This workshop would not have been possible without the support and dedication of the following individuals:

**Associate Director of Education**
- Denise Yoon

**Teaching Assistants** (listed alphabetically)
- Bala Desinghu
- Yasin Mazloumi
- Nihal Vivekanand Nayak
- Timothy Ngotiaoco

Their expertise and commitment to helping participants navigate the hands-on labs made this workshop a success.

---

<div style="text-align: center; margin: 30px 0;">
  <img src="/images/news/vllm-workshop-2026/2026-vllm-workshop-attendees.png" alt="vLLM Workshop Attendees" style="max-width: 800px; width: 100%; height: auto; border-radius: 8px;" />
</div>

**Workshop Flyer:** [Download PDF](/images/news/vllm-workshop-2026/Workshop-3-26-26-Flyer-2.pdf)


