---
id: gpu/apple-m3-max
type: gpu
slug: apple-m3-max
schema_version: 1.1
title: M3 Max
vendor: Apple
segment: workstation
series: Apple Silicon
generation: M3
release_date: '2023-10-30'
signal_strength: medium
summary: 3nm laptop chip with up to 128GB unified memory. Best portable platform for local LLM inference.
aliases:
- Apple M3 Max
specifications:
  memory_gb: 128
  memory_type: LPDDR5
  memory_kind: unified
  memory_bandwidth_gb_per_s: 400
  unit_kind: gpu
  compute_units: 40
  compute_unit_type: GPU Cores
  tdp_watts: 40
  form_factor:
  - SoC (MacBook Pro / Mac Studio)
  process_node:
    nodes_nm:
    - 3
performance:
  fp32_tflops: 14.2
  fp16_tflops: 28.4
ml_capabilities:
  inference: true
  training: false
  fine_tuning: true
  max_model_params_b_inference: 65
  sparsity_support: false
  transformer_engine: false
framework_support:
  pytorch: true
  tensorflow: true
  jax: true
  onnx_runtime: true
  tensorrt: false
  directml: false
  mlx: true
  rocm: false
  oneapi: false
  triton: false
  vllm: false
  deepspeed: false
market:
  msrp_usd: 3199
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Laptop-based ML inference
- MLX development
- Portable AI workstation
key_features:
- Up to 128 GB unified memory
- 3nm process
- 40 GPU cores
- Neural Engine (16 cores)
limitations:
- Lower bandwidth than Ultra chips
- 40 GPU cores limits throughput
- Consumer pricing
notable_users:
- Developers on MacBook Pro
image: /images/gpus/apple-m3-max.jpg
tags:
- apple
- workstation
- m3
updated: '2026-11-19'
sources: []
---

## Overview

3nm laptop chip with up to 128GB unified memory. Best portable platform for local LLM inference.
