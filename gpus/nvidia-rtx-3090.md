---
id: gpu/nvidia-rtx-3090
type: gpu
slug: nvidia-rtx-3090
schema_version: 1.3
title: GeForce RTX 3090
vendor: NVIDIA
segment: consumer
series: GeForce RTX 30
generation: Ampere
release_date: '2020-09-24'
signal_strength: low
summary: Previous-gen 24GB consumer GPU. Strong used market presence for budget AI enthusiasts.
aliases:
- NVIDIA GeForce RTX 3090
specifications:
  memory_gb: 24
  memory_type: GDDR6X
  memory_bandwidth_gb_per_s: 936
  unit_kind: gpu
  compute_units: 10496
  compute_unit_type: CUDA Cores
  tensor_cores: 328
  rt_cores: 82
  tdp_watts: 350
  form_factor:
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: NVLink
    note: SLI
  process_node:
    nodes_nm:
    - 8
performance:
  fp32_tflops: 35.6
  fp16_tflops: 71.0
  bf16_tflops: 71.0
  tf32_tflops: 71.0
  int8_tops: 284.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 13
  max_model_params_b_training: 3
  sparsity_support: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: NVLink
    max_units: 2
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
  deepspeed: true
market:
  msrp_usd: 1499
  msrp_source: https://nvidianews.nvidia.com/news/nvidia-delivers-greatest-ever-generational-leap-in-performance-with-geforce-rtx-30-series-gpus
  msrp_announced: '2020-09-01'
  cloud_hourly_usd: 0.22
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Budget local AI
- Used market value
- Hobbyist training
key_features:
- 24 GB GDDR6X
- NVLink for 2-GPU SLI
- Good used market availability
- Ampere architecture
limitations:
- No FP8
- Older generation
- High power draw for performance
notable_users:
- ML hobbyists
- Used GPU market
image: /images/gpus/nvidia-rtx-3090.jpg
tags:
- nvidia
- consumer
- ampere
updated: '2026-11-21'
sources:
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

Previous-gen 24GB consumer GPU. Strong used market presence for budget AI enthusiasts.
