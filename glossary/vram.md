---
id: glossary-term/vram
type: glossary-term
slug: vram
schema_version: 3.0
title: VRAM (Video Memory)
term: VRAM (Video Memory)
category: memory
examples:
- 24 GB GDDR6X on GeForce RTX 4090
- 80 GB on H100 SXM
- 192 GB HBM3 on Instinct MI300X
related:
- glossary-term/hbm
- glossary-term/gddr6
- glossary-term/memory-bandwidth
tags:
- memory
- vram
- capacity
updated: '2026-11-21'
sources:
- url: https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/
  title: 'Mastering LLM Techniques: Inference Optimization (NVIDIA)'
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/
  title: GeForce RTX 4090 specifications (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU (NVIDIA)
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html
  title: AMD Instinct MI300X Accelerators (AMD)
  trust: 0.95
---

## Definition

VRAM is the memory attached to the GPU (HBM on datacenter accelerators, GDDR on consumer cards). For
AI it holds what the GPU works on; NVIDIA names the model parameters and the KV cache (cached attention
tensors) as the main occupants during inference.

## Why You Care

If the weights plus working memory do not fit, the job fails or must be split across GPUs. NVIDIA
estimates weights as parameters × bytes per parameter (7B × 2 bytes in FP16 ≈ 14 GB). By the same
arithmetic a 70B model in FP16 needs about 140 GB for weights alone, more than a 24 GB card holds.
