---
id: gpu/nvidia-h200
type: gpu
slug: nvidia-h200
schema_version: 1.1
title: H200
vendor: NVIDIA
segment: datacenter
series: Hopper
generation: Hopper
release_date: '2024-04-01'
signal_strength: high
summary: Memory-upgraded H100 with 141GB HBM3e. Ideal for LLM inference where memory capacity is the bottleneck.
aliases:
- NVIDIA H200
specifications:
  memory_gb: 141
  memory_type: HBM3e
  memory_bandwidth_gb_per_s: 4800
  unit_kind: gpu
  compute_units: 16896
  compute_unit_type: CUDA Cores
  tensor_cores: 528
  tdp_watts: 700
  form_factor:
  - SXM5
  pcie_gen: 5.0
  interconnect:
    name: NVLink 4.0
    bandwidth_gb_per_s: 900
  process_node:
    nodes_nm:
    - 4
performance:
  fp32_tflops: 67.0
  fp16_tflops: 989.0
  bf16_tflops: 989.0
  tf32_tflops: 495.0
  fp8_tflops: 1979.0
  int8_tops: 1979.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 140
  max_model_params_b_training: 50
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: NVLink + NVSwitch
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
  cloud_hourly_usd: 4.75
  cloud_providers:
  - name: AWS
  - name: GCP
  - name: Azure
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- LLM inference with long contexts
- Large model training
- Serving 70B+ models on single GPU
key_features:
- 141 GB HBM3e (76% more than H100)
- 4.8 TB/s memory bandwidth
- Same compute as H100 SXM
- Ideal for large-context LLM inference
limitations:
- High power consumption (700W)
- Requires liquid cooling
- Premium pricing
notable_users:
- OpenAI
- Google Cloud
- Meta
- Microsoft Azure
image: /images/gpus/nvidia-h200.jpg
tags:
- nvidia
- datacenter
- hopper
updated: '2026-11-21'
sources:
- url: https://getdeploying.com/dataset/gpu-models/gpu-models.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

Memory-upgraded H100 with 141GB HBM3e. Ideal for LLM inference where memory capacity is the bottleneck.
