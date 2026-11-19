---
id: gpu/nvidia-b200
type: gpu
slug: nvidia-b200
schema_version: 1.1
title: B200
vendor: NVIDIA
segment: datacenter
series: Blackwell
generation: Blackwell
release_date: '2025-01-01'
signal_strength: high
summary: NVIDIA's highest-performance Blackwell GPU with dual-die design, targeting frontier AI workloads.
aliases:
- NVIDIA B200
specifications:
  memory_gb: 192
  memory_type: HBM3e
  memory_bandwidth_gb_per_s: 8000
  unit_kind: gpu
  compute_units: 18432
  compute_unit_type: CUDA Cores
  tensor_cores: 576
  tdp_watts: 1000
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
  fp32_tflops: 90.0
  fp16_tflops: 2250.0
  bf16_tflops: 2250.0
  tf32_tflops: 1125.0
  fp8_tflops: 4500.0
  int8_tops: 4500.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 175
  max_model_params_b_training: 80
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
  msrp_usd: 50000
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Frontier model training
- Multi-trillion parameter models
- Massive-scale inference
key_features:
- Dual-die Blackwell GPU
- 4.5 PetaFLOPS FP8 performance
- 192 GB HBM3e
- NVLink 5.0 (1.8 TB/s)
limitations:
- 1000W TDP
- Requires advanced cooling
- Extremely expensive
notable_users:
- Hyperscalers
- AI research labs
image: /images/gpus/nvidia-b200.jpg
tags:
- nvidia
- datacenter
- blackwell
updated: '2026-11-19'
sources: []
---

## Overview

NVIDIA's highest-performance Blackwell GPU with dual-die design, targeting frontier AI workloads.
