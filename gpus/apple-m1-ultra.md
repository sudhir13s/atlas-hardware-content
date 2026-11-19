---
id: gpu/apple-m1-ultra
type: gpu
slug: apple-m1-ultra
schema_version: 1.1
title: M1 Ultra
vendor: Apple
segment: workstation
series: Apple Silicon
generation: M1
release_date: '2022-03-08'
signal_strength: low
summary: Apple's first ultra-tier chip. 128GB unified memory lets it run large models locally despite lower raw compute.
aliases:
- Apple M1 Ultra
specifications:
  memory_gb: 128
  memory_type: LPDDR5
  memory_kind: unified
  memory_bandwidth_gb_per_s: 800
  unit_kind: gpu
  compute_units: 64
  compute_unit_type: GPU Cores
  tdp_watts: 60
  form_factor:
  - SoC (Mac Studio / Mac Pro)
  interconnect:
    name: UltraFusion
    bandwidth_gb_per_s: 2500
    note: 2.5 TB/s die-to-die
  process_node:
    nodes_nm:
    - 5
performance:
  fp32_tflops: 21.2
  fp16_tflops: 42.4
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
  msrp_usd: 3999
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Local LLM inference (large models fit in unified memory)
- Mac-native ML development
- Power-efficient AI
key_features:
- 128 GB unified memory (CPU + GPU shared)
- UltraFusion die-to-die interconnect
- Neural Engine (32 cores)
- Extremely power efficient
limitations:
- Low raw compute vs NVIDIA
- Limited training capability
- Apple ecosystem lock-in
notable_users:
- Mac ML developers
- Indie researchers
image: /images/gpus/apple-m1-ultra.jpg
tags:
- apple
- workstation
- m1
updated: '2026-11-19'
sources: []
---

## Overview

Apple's first ultra-tier chip. 128GB unified memory lets it run large models locally despite lower raw compute.
