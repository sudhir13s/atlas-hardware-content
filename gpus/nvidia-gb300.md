---
id: gpu/nvidia-gb300
type: gpu
slug: nvidia-gb300
schema_version: 1.1
title: GB300 Grace Blackwell Ultra Superchip
vendor: NVIDIA
segment: datacenter
series: Blackwell Ultra
generation: Blackwell Ultra
release_date: '2025-06-01'
signal_strength: high
summary: NVIDIA's top-tier superchip with Blackwell Ultra GPUs and significantly expanded memory, for the largest AI workloads.
aliases:
- NVIDIA GB300 Grace Blackwell Ultra Superchip
specifications:
  memory_gb: 576
  memory_type: HBM3e + LPDDR5X
  memory_note: 288GB per GPU
  memory_bandwidth_gb_per_s: 24000
  unit_kind: module
  gpus_per_module: 2
  compute_units: 40960
  compute_unit_type: CUDA Cores
  compute_unit_note: 2x Blackwell Ultra GPUs
  tensor_cores: 1280
  tdp_watts: 2900
  form_factor:
  - Superchip Module
  pcie_gen: 6.0
  interconnect:
    name: NVLink 5.0 + Grace CPU coherent link
    bandwidth_gb_per_s: 1800
    note: 1800 GB/s per GPU
  process_node:
    nodes_nm:
    - 4
performance:
  fp32_tflops: 200.0
  fp16_tflops: 5000.0
  bf16_tflops: 5000.0
  tf32_tflops: 2500.0
  fp8_tflops: 10000.0
  int8_tops: 10000.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 600
  max_model_params_b_training: 250
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
  cloud_hourly_usd: 18.0
  observed_at: '2026-11-20'
  source: GetDeploying GPU cloud prices
best_for:
- Next-generation frontier models
- Massive-scale training clusters
- Ultra-large context inference
key_features:
- Blackwell Ultra GPUs with 288GB HBM3e each
- 576 GB total memory per superchip
- Enhanced NVLink bandwidth
- FP4 inference acceleration
limitations:
- Extreme power requirements
- Not yet widely available
- Highest cost tier
notable_users:
- AI hyperscalers
image: /images/gpus/nvidia-gb300.jpg
tags:
- nvidia
- datacenter
- blackwell-ultra
updated: '2026-11-20'
sources:
- url: https://getdeploying.com/dataset/gpu-models/gpu-models.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

NVIDIA's top-tier superchip with Blackwell Ultra GPUs and significantly expanded memory, for the largest AI workloads.
