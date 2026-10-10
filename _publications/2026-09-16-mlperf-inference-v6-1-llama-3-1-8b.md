---
title: "MLPerf Inference v6.1: Llama 3.1-8B in FP8 on a single NVIDIA H200 (Closed Division, Datacenter)"
collection: publications
category: datasets
permalink: /publication/2026-09-16-mlperf-inference-v6-1-llama-3-1-8b
excerpt: 'An audited, peer-reviewed MLPerf Inference v6.1 submission: Llama 3.1-8B with FP8 weights, activations and KV cache through TensorRT-LLM on one NVIDIA H200 SXM 141 GB, measuring 7,796.59 output tokens/s Offline and 7,376.60 output tokens/s Server within the p99 latency limits, with the full configuration and accuracy artifacts published in the MLCommons results repository.'
date: 2026-09-16
venue: 'MLCommons MLPerf Inference v6.1 results (Closed Division, Datacenter), individual submitter'
paperurl: 'https://github.com/mlcommons/inference_results_v6.1/tree/main/closed/Naeem%20Khoshnevis'
citation: 'Khoshnevis, N. (2026). MLPerf Inference v6.1 results: Llama 3.1-8B, FP8, 1x NVIDIA H200 SXM 141 GB, Closed Division, Datacenter. MLCommons. https://mlcommons.org/2026/09/mlperf-inference-v6-1-results/'
---

## Summary

A single NVIDIA H200 SXM 141 GB accelerator ran Llama 3.1-8B with FP8 weights, activations and KV cache (NVIDIA ModelOpt post-training quantization with static per-tensor scaling) through TensorRT-LLM 1.0.0 and `trtllm-serve`, driven by the MLCommons endpoints harness over HTTP.

| Scenario | Result | Constraint |
|---|---|---|
| Offline | 7,796.59 output tokens/s over 40,104 queries in 658.34 s | aggregate throughput |
| Server | 7,376.60 output tokens/s at target QPS 58; p99 TTFT 1,495.94 ms, p99 TPOT 61.22 ms | TTFT under 2,000 ms, TPOT under 100 ms |

All 13,368 CNN/DailyMail validation examples were scored in both scenarios with zero empty or failed responses, and every ROUGE metric cleared the required floor (ROUGE1 38.64 against 38.39, ROUGE2 15.93 against 15.75, ROUGEL 24.50 against 24.25, ROUGELSUM 35.74 against 35.44). The results were published by MLCommons on 2026-09-16; the complete submission, including system and benchmark configuration, calibration documentation and accuracy artifacts, is in the [MLCommons results repository](https://github.com/mlcommons/inference_results_v6.1/tree/main/closed/Naeem%20Khoshnevis).

The [technical write-up](/news/2026-09-16-mlperf-inference-v6-1/) covers quantization and calibration, Server operating-point selection, the endpoints harness, cross-request KV reuse, and the operating-system and network details that had to be controlled for a valid, reproducible result.
