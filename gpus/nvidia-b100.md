---
id: gpu/nvidia-b100
type: gpu
slug: nvidia-b100
schema_version: 1.1
title: B100
vendor: NVIDIA
segment: datacenter
series: Blackwell
generation: Blackwell
release_date: '2024-11-01'
signal_strength: high
summary: NVIDIA Blackwell GPU with massive memory and bandwidth upgrades over Hopper, targeting frontier model training.
aliases:
- NVIDIA B100
specifications:
  memory_gb: 192
  memory_type: HBM3e
  memory_bandwidth_gb_per_s: 8000
  unit_kind: gpu
  compute_units: 18432
  compute_unit_type: CUDA Cores
  tensor_cores: 576
  tdp_watts: 700
  form_factor:
  - SXM
  pcie_gen: 5.0
  interconnect:
    name: NVLink 5.0
    bandwidth_gb_per_s: 1800
  process_node:
    nodes_nm:
    - 4
performance:
  fp32_tflops: 80.0
  fp16_tflops: 1800.0
  bf16_tflops: 1800.0
  tf32_tflops: 900.0
  fp8_tflops: 3500.0
  int8_tops: 3500.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 175
  max_model_params_b_training: 70
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: NVLink 5.0 + NVSwitch
framework_support:
  pytorch: true
  tensorflow: true
  jax: true
  onnx_runtime: true
  tensorrt: true
  directml: false
  mlx: false
  rocm: false
  oneapi: false
  triton: true
  vllm: true
  deepspeed: true
market:
  msrp_usd: 40000
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Next-gen LLM training
- Large-scale inference
- Frontier model development
key_features:
- 2nd-gen Transformer Engine
- 192 GB HBM3e
- NVLink 5.0 (1.8 TB/s)
- FP4 support for inference
limitations:
- Very expensive
- High power draw
- Limited initial availability
notable_users:
- OpenAI
- Meta
- Google
- xAI
image: /images/gpus/nvidia-b100.jpg
tags:
- nvidia
- datacenter
- blackwell
updated: '2026-11-19'
sources: []
---

## Overview

NVIDIA Blackwell GPU with massive memory and bandwidth upgrades over Hopper, targeting frontier model training.
