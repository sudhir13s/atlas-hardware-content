---
id: gpu/nvidia-l40
type: gpu
slug: nvidia-l40
schema_version: 1.1
title: L40
vendor: NVIDIA
segment: datacenter
series: Ada Lovelace
generation: Ada Lovelace
release_date: '2023-03-21'
signal_strength: low
summary: Datacenter GPU for combined AI inference and professional graphics workloads.
aliases:
- NVIDIA L40
specifications:
  memory_gb: 48
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 864
  unit_kind: gpu
  compute_units: 18176
  compute_unit_type: CUDA Cores
  tensor_cores: 568
  rt_cores: 142
  tdp_watts: 300
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 5
performance:
  fp32_tflops: 90.5
  fp16_tflops: 181.0
  bf16_tflops: 181.0
  tf32_tflops: 181.0
  int8_tops: 724.0
ml_capabilities:
  inference: true
  training: false
  fine_tuning: true
  max_model_params_b_inference: 25
  sparsity_support: true
  transformer_engine: false
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
  deepspeed: false
market:
  msrp_usd: 8000
  cloud_hourly_usd: 1.0
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- AI inference + rendering
- Virtual workstations
- Media and entertainment AI
key_features:
- 48 GB GDDR6
- Optimized for graphics + AI
- Full RT cores for rendering
- Lower TDP than L40S
limitations:
- No FP8 Transformer Engine
- Not designed for training
notable_users:
- Enterprise VDI
- Media companies
image: /images/gpus/nvidia-l40.jpg
tags:
- nvidia
- datacenter
- ada-lovelace
updated: '2026-11-20'
sources:
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

Datacenter GPU for combined AI inference and professional graphics workloads.
