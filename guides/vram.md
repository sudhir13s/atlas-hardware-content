---
id: guide/vram
type: guide
slug: vram
schema_version: 1.1
title: 'VRAM: The Most Important Spec for AI'
order: 1
vram_by_model_size:
- model_size: 1-3B
  fp16: 2-6 GB
  int8: 1-3 GB
  int4: 0.5-1.5 GB
  recommended_gpu: Any GPU with 4GB+
- model_size: 7B
  fp16: 14 GB
  int8: 7 GB
  int4: 4 GB
  recommended_gpu: RTX 3080/4070 (8-16GB)
- model_size: 13B
  fp16: 26 GB
  int8: 13 GB
  int4: 7 GB
  recommended_gpu: RTX 4090 (24GB)
- model_size: 34B
  fp16: 68 GB
  int8: 34 GB
  int4: 18 GB
  recommended_gpu: RTX 4090 (4-bit) or A100 40GB
- model_size: 70B
  fp16: 140 GB
  int8: 70 GB
  int4: 35-40 GB
  recommended_gpu: A100 80GB / MI300X / M4 Ultra
- model_size: 405B
  fp16: 810 GB
  int8: 405 GB
  int4: ~200 GB
  recommended_gpu: Multi-GPU cluster (8×H100)
rules_of_thumb:
- 7B model at FP16 = ~14GB VRAM
- 7B model at 4-bit = ~4GB VRAM
- 13B model at FP16 = ~26GB VRAM
- 70B model at 4-bit = ~40GB VRAM
- 70B model at FP16 = ~140GB VRAM
tags:
- gpu-buying-guide
- vram
updated: '2026-11-19'
sources: []
---

## Overview

For LLM inference, VRAM determines the largest model you can run. For training, it determines your batch size. Everything else is secondary.

## Takeaway

Formula: VRAM needed ≈ parameters × bytes per param. FP16 = 2 bytes, INT8 = 1 byte, 4-bit = 0.5 bytes. Add ~10-20% overhead for KV cache and activations.
