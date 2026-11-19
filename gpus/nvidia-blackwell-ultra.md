---
id: gpu/nvidia-blackwell-ultra
type: gpu
slug: nvidia-blackwell-ultra
schema_version: 1.1
title: Blackwell Ultra B300
vendor: NVIDIA
segment: datacenter
series: Blackwell Ultra
generation: Blackwell Ultra
release_date: '2025-06-01'
signal_strength: high
summary: NVIDIA's Blackwell Ultra standalone GPU with 288GB HBM3e, the single-GPU memory champion for AI workloads.
aliases:
- NVIDIA Blackwell Ultra B300
specifications:
  memory_gb: 288
  memory_type: HBM3e
  memory_bandwidth_gb_per_s: 12000
  unit_kind: gpu
  compute_units: 20480
  compute_unit_type: CUDA Cores
  tensor_cores: 640
  tdp_watts: 1200
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
  fp32_tflops: 100.0
  fp16_tflops: 2500.0
  bf16_tflops: 2500.0
  tf32_tflops: 1250.0
  fp8_tflops: 5000.0
  int8_tops: 5000.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 250
  max_model_params_b_training: 100
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
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Frontier model training
- Ultra-large model inference
- Next-gen AI research
key_features:
- 288 GB HBM3e per GPU
- 12 TB/s memory bandwidth
- Enhanced Transformer Engine
- FP4 support for maximum inference throughput
limitations:
- Extreme power draw
- Requires rack-scale liquid cooling
- Premium pricing
notable_users:
- AI research labs
- Hyperscale cloud providers
image: /images/gpus/nvidia-blackwell-ultra.jpg
tags:
- nvidia
- datacenter
- blackwell-ultra
updated: '2026-11-19'
sources: []
---

## Overview

NVIDIA's Blackwell Ultra standalone GPU with 288GB HBM3e, the single-GPU memory champion for AI workloads.
