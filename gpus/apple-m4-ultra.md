---
id: gpu/apple-m4-ultra
type: gpu
slug: apple-m4-ultra
schema_version: 1.1
title: M4 Ultra
vendor: Apple
segment: workstation
series: Apple Silicon
generation: M4
release_date: '2025-03-01'
signal_strength: high
summary: Apple's most powerful chip with 256GB unified memory. Can run 175B+ parameter models locally via MLX.
aliases:
- Apple M4 Ultra
specifications:
  memory_gb: 256
  memory_type: LPDDR5X
  memory_kind: unified
  memory_bandwidth_gb_per_s: 1092
  unit_kind: gpu
  compute_units: 80
  compute_unit_type: GPU Cores
  tdp_watts: 75
  form_factor:
  - SoC (Mac Studio / Mac Pro)
  interconnect:
    name: UltraFusion
  process_node:
    nodes_nm:
    - 3
    note: 3nm (2nd gen)
performance:
  fp32_tflops: 36.0
  fp16_tflops: 72.0
ml_capabilities:
  inference: true
  training: false
  fine_tuning: true
  max_model_params_b_inference: 175
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
  msrp_usd: 5999
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Running 100B+ models locally
- MLX inference at scale
- Desktop AI workstation
key_features:
- 256 GB unified LPDDR5X
- 80 GPU cores
- 1 TB/s+ memory bandwidth
- Neural Engine (32 cores)
- UltraFusion die-to-die
limitations:
- Low raw compute vs NVIDIA datacenter
- Apple ecosystem
- High price for compute ratio
notable_users:
- Mac AI power users
- Researchers needing local large model access
image: /images/gpus/apple-m4-ultra.jpg
tags:
- apple
- workstation
- m4
updated: '2026-11-19'
sources: []
---

## Overview

Apple's most powerful chip with 256GB unified memory. Can run 175B+ parameter models locally via MLX.
