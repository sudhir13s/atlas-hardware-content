---
id: gpu/nvidia-l4
type: gpu
slug: nvidia-l4
schema_version: 1.1
title: L4
vendor: NVIDIA
segment: datacenter
series: Ada Lovelace
generation: Ada Lovelace
release_date: '2023-03-21'
signal_strength: medium
summary: Ultra-efficient inference GPU. 72W power draw makes it ideal for dense, cost-sensitive inference deployments.
aliases:
- NVIDIA L4
specifications:
  memory_gb: 24
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 300
  unit_kind: gpu
  compute_units: 7424
  compute_unit_type: CUDA Cores
  tensor_cores: 232
  rt_cores: 58
  tdp_watts: 72
  form_factor:
  - PCIe (low-profile)
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 5
performance:
  fp32_tflops: 30.3
  fp16_tflops: 60.6
  bf16_tflops: 60.6
  tf32_tflops: 60.6
  fp8_tflops: 242.0
  int8_tops: 242.0
ml_capabilities:
  inference: true
  training: false
  fine_tuning: false
  max_model_params_b_inference: 13
  sparsity_support: true
  transformer_engine: true
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
  msrp_usd: 2500
  cloud_hourly_usd: 0.7946
  cloud_providers:
  - name: GCP
    instance_note: g2 instances
  - name: AWS
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- High-density inference
- Edge AI deployment
- Cost-effective serving of 7B models
key_features:
- Ultra-low power (72W)
- Low-profile PCIe form factor
- FP8 Transformer Engine
- Fits in any server
limitations:
- 24GB limits model size
- Low memory bandwidth
- Inference only
notable_users:
- GCP g2 instances
- Edge deployments
- Inference services
image: /images/gpus/nvidia-l4.jpg
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

Ultra-efficient inference GPU. 72W power draw makes it ideal for dense, cost-sensitive inference deployments.
