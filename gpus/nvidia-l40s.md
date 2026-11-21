---
id: gpu/nvidia-l40s
type: gpu
slug: nvidia-l40s
schema_version: 1.1
title: L40S
vendor: NVIDIA
segment: datacenter
series: Ada Lovelace
generation: Ada Lovelace
release_date: '2023-10-17'
signal_strength: medium
summary: Versatile datacenter GPU bridging AI inference and graphics workloads with 48GB and FP8 support.
aliases:
- NVIDIA L40S
specifications:
  memory_gb: 48
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 864
  unit_kind: gpu
  compute_units: 18176
  compute_unit_type: CUDA Cores
  tensor_cores: 568
  rt_cores: 142
  tdp_watts: 350
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 5
performance:
  fp32_tflops: 91.6
  fp16_tflops: 183.0
  bf16_tflops: 183.0
  tf32_tflops: 183.0
  fp8_tflops: 733.0
  int8_tops: 733.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 25
  max_model_params_b_training: 10
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
  deepspeed: true
market:
  cloud_hourly_usd: 1.8
  cloud_providers:
  - name: AWS
    instance_note: g6e
  - name: GCP
  - name: Azure
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Inference at scale
- Fine-tuning medium models
- AI + video processing
- Generative AI inference
key_features:
- 48 GB GDDR6 with ECC
- FP8 Transformer Engine
- Combined AI + Graphics/Video
- Ada Lovelace architecture
limitations:
- GDDR6 bandwidth lower than HBM
- No NVLink
- Not ideal for large-scale training
notable_users:
- Cloud providers
- Media companies
- Inference services
image: /images/gpus/nvidia-l40s.jpg
tags:
- nvidia
- datacenter
- ada-lovelace
updated: '2026-11-21'
sources:
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

Versatile datacenter GPU bridging AI inference and graphics workloads with 48GB and FP8 support.
