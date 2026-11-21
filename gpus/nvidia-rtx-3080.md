---
id: gpu/nvidia-rtx-3080
type: gpu
slug: nvidia-rtx-3080
schema_version: 1.3
title: GeForce RTX 3080
vendor: NVIDIA
segment: consumer
series: GeForce RTX 30
generation: Ampere
release_date: '2020-09-17'
signal_strength: low
summary: Budget Ampere consumer GPU. 10GB VRAM is too limited for most modern LLM workloads.
aliases:
- NVIDIA GeForce RTX 3080
specifications:
  memory_gb: 10
  memory_type: GDDR6X
  memory_bandwidth_gb_per_s: 760
  unit_kind: gpu
  compute_units: 8704
  compute_unit_type: CUDA Cores
  tensor_cores: 272
  rt_cores: 68
  tdp_watts: 320
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 8
performance:
  fp32_tflops: 29.8
  fp16_tflops: 59.6
  bf16_tflops: 59.6
  tf32_tflops: 59.6
  int8_tops: 238.0
ml_capabilities:
  inference: true
  training: false
  fine_tuning: false
  max_model_params_b_inference: 3
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
  vllm: false
  deepspeed: false
market:
  msrp_usd: 699
  msrp_source: https://nvidianews.nvidia.com/news/nvidia-delivers-greatest-ever-generational-leap-in-performance-with-geforce-rtx-30-series-gpus
  msrp_announced: '2020-09-01'
  cloud_hourly_usd: 0.14
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Small model inference
- ML learning and experimentation
key_features:
- 10 GB GDDR6X
- Good value on used market
- Ampere architecture
limitations:
- 10GB severely limits LLM use
- No NVLink
- No FP8
notable_users:
- Hobbyists
- Students
image: /images/gpus/nvidia-rtx-3080.jpg
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

Budget Ampere consumer GPU. 10GB VRAM is too limited for most modern LLM workloads.
