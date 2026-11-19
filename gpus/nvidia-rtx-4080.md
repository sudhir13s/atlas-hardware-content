---
id: gpu/nvidia-rtx-4080
type: gpu
slug: nvidia-rtx-4080
schema_version: 1.1
title: GeForce RTX 4080
vendor: NVIDIA
segment: consumer
series: GeForce RTX 40
generation: Ada Lovelace
release_date: '2022-11-16'
signal_strength: low
summary: Mid-range consumer GPU. Useful for quantized model inference but 16GB limits LLM capabilities.
aliases:
- NVIDIA GeForce RTX 4080
specifications:
  memory_gb: 16
  memory_type: GDDR6X
  memory_bandwidth_gb_per_s: 717
  unit_kind: gpu
  compute_units: 9728
  compute_unit_type: CUDA Cores
  tensor_cores: 304
  rt_cores: 76
  tdp_watts: 320
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 5
performance:
  fp32_tflops: 48.7
  fp16_tflops: 97.5
  bf16_tflops: 97.5
  tf32_tflops: 97.5
  fp8_tflops: 390.0
  int8_tops: 390.0
ml_capabilities:
  inference: true
  training: false
  fine_tuning: true
  max_model_params_b_inference: 7
  sparsity_support: true
  transformer_engine: false
framework_support:
  pytorch: true
  tensorflow: true
  jax: true
  onnx_runtime: true
  tensorrt: true
  directml: true
  mlx: false
  rocm: false
  oneapi: false
  triton: true
  vllm: true
  deepspeed: false
market:
  msrp_usd: 1199
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Local inference of quantized models
- Light fine-tuning
- ML experimentation
key_features:
- 16 GB GDDR6X
- Good price-performance for inference
- Ada Lovelace architecture
limitations:
- 16GB very limiting for LLMs
- No NVLink
- Consumer only
notable_users:
- Hobbyists
- Small teams
image: /images/gpus/nvidia-rtx-4080.jpg
tags:
- nvidia
- consumer
- ada-lovelace
updated: '2026-11-19'
sources: []
---

## Overview

Mid-range consumer GPU. Useful for quantized model inference but 16GB limits LLM capabilities.
