---
id: gpu/intel-arc-a770
type: gpu
slug: intel-arc-a770
schema_version: 1.1
title: Arc A770
vendor: Intel
segment: consumer
series: Arc
generation: Alchemist
release_date: '2022-10-12'
signal_strength: low
summary: Intel's consumer GPU with 16GB VRAM. Cheap entry point but limited ML framework support.
aliases:
- Intel Arc A770
specifications:
  memory_gb: 16
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 560
  unit_kind: gpu
  compute_units: 32
  compute_unit_type: Xe Cores
  rt_cores: 32
  tdp_watts: 225
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 6
performance:
  fp32_tflops: 19.7
  fp16_tflops: 39.3
  int8_tops: 157.0
ml_capabilities:
  inference: true
  training: false
  fine_tuning: false
  max_model_params_b_inference: 7
  sparsity_support: false
  transformer_engine: false
framework_support:
  pytorch: true
  tensorflow: true
  jax: false
  onnx_runtime: true
  tensorrt: false
  directml: true
  mlx: false
  rocm: false
  oneapi: true
  triton: false
  vllm: false
  deepspeed: false
market:
  msrp_usd: 349
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Budget AI experimentation
- oneAPI development
- Small model inference
key_features:
- 16 GB GDDR6
- XMX (Xe Matrix Extensions) for AI
- Affordable entry point
- oneAPI support
limitations:
- Very limited ML ecosystem
- Driver maturity issues
- Low performance for serious ML
notable_users:
- Hobbyists
- oneAPI developers
image: /images/gpus/intel-arc-a770.jpg
tags:
- intel
- consumer
- alchemist
updated: '2026-11-19'
sources: []
---

## Overview

Intel's consumer GPU with 16GB VRAM. Cheap entry point but limited ML framework support.
