---
id: glossary-term/memory-bandwidth
type: glossary-term
slug: memory-bandwidth
schema_version: 3.0
title: Memory Bandwidth
term: Memory Bandwidth
category: memory
examples:
- 3.35 TB/s on H100 SXM (HBM3)
- Up to 960 GB/s on Radeon RX 7900 XTX (GDDR6)
- 5.3 TB/s peak on Instinct MI300X (HBM3)
related:
- glossary-term/hbm
- glossary-term/vram
tags:
- memory
- bandwidth
- performance
updated: '2026-11-21'
sources:
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html
  title: AMD Instinct MI300X Accelerators (AMD)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/
  title: NVIDIA Hopper Architecture In-Depth (NVIDIA)
  trust: 0.95
- url: https://www.amd.com/en/products/graphics/desktops/radeon/7000-series/amd-radeon-rx-7900xtx.html
  title: Radeon RX 7900 XTX specifications (AMD)
  trust: 0.95
- url: https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/
  title: 'Mastering LLM Techniques: Inference Optimization (NVIDIA)'
  trust: 0.95
---

## Definition

Memory bandwidth is the rate at which data moves between the GPU and its memory, in GB/s or TB/s.
Peak bandwidth is bus width times per-pin data rate, divided by 8: AMD computes 8,192 bits × 5.2 Gbps
/ 8 = 5.325 TB/s for the Instinct MI300X.

## Why You Care

NVIDIA states that the token-generation (decode) phase of large-language-model inference is memory
bound: the speed of moving weights and cached values from memory dominates latency. Two cards with
similar TFLOPS can therefore generate tokens at different speeds.
