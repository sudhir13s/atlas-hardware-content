---
id: gpu/nvidia-rtx-4090
type: gpu
slug: nvidia-rtx-4090
schema_version: 1.3
title: GeForce RTX 4090
vendor: NVIDIA
segment: consumer
series: GeForce RTX 40
generation: Ada Lovelace
release_date: '2022-10-12'
signal_strength: medium
summary: Previous-gen flagship consumer GPU. Excellent for local AI work with 24GB VRAM and strong FP8.
aliases:
- NVIDIA GeForce RTX 4090
specifications:
  memory_gb: 24
  memory_type: GDDR6X
  memory_bandwidth_gb_per_s: 1008
  unit_kind: gpu
  compute_units: 16384
  compute_unit_type: CUDA Cores
  tensor_cores: 512
  rt_cores: 128
  tdp_watts: 450
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 5
performance:
  fp32_tflops: 82.6
  fp16_tflops: 165.2
  bf16_tflops: 165.2
  tf32_tflops: 165.2
  fp8_tflops: 660.6
  int8_tops: 660.6
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 13
  max_model_params_b_training: 5
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
  vllm: true
  deepspeed: true
market:
  msrp_usd: 1599
  msrp_source: https://nvidianews.nvidia.com/news/nvidia-delivers-quantum-leap-in-performance-introduces-new-era-of-neural-rendering-with-geforce-rtx-40-series
  msrp_announced: '2022-09-20'
  cloud_hourly_usd: 0.456
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Local LLM inference
- Fine-tuning 7B models
- ML prototyping
- Gaming + AI
key_features:
- 24 GB GDDR6X
- Excellent FP8 performance
- Best previous-gen consumer GPU for AI
- DLSS 3
limitations:
- 24GB limits model size
- Consumer drivers
- No NVLink
- No ECC
notable_users:
- ML hobbyists
- Independent researchers
- Small startups
image: /images/gpus/nvidia-rtx-4090.jpg
tags:
- nvidia
- consumer
- ada-lovelace
updated: '2026-11-21'
sources:
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

Previous-gen flagship consumer GPU. Excellent for local AI work with 24GB VRAM and strong FP8.
