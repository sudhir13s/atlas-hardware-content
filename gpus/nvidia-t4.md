---
id: gpu/nvidia-t4
type: gpu
slug: nvidia-t4
schema_version: 1.1
title: T4
vendor: NVIDIA
segment: datacenter
series: Turing
generation: Turing
release_date: '2018-09-13'
signal_strength: low
summary: Budget-friendly inference GPU. Still widely deployed but increasingly dated for modern LLM workloads.
aliases:
- NVIDIA T4
specifications:
  memory_gb: 16
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 320
  unit_kind: gpu
  compute_units: 2560
  compute_unit_type: CUDA Cores
  tensor_cores: 320
  tdp_watts: 70
  form_factor:
  - PCIe (low-profile)
  pcie_gen: 3.0
  process_node:
    nodes_nm:
    - 12
performance:
  fp32_tflops: 8.1
  fp16_tflops: 65.0
  int8_tops: 130.0
ml_capabilities:
  inference: true
  training: false
  fine_tuning: false
  max_model_params_b_inference: 7
  sparsity_support: false
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
  cloud_hourly_usd: 0.752
  cloud_providers:
  - name: AWS
    instance_note: g4dn
  - name: GCP
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Budget inference
- Batch processing
- Small model serving
key_features:
- Ultra-low power (70W)
- Cheapest NVIDIA inference GPU
- Widely available on all clouds
- INT8 inference acceleration
limitations:
- 16GB only
- Older architecture
- No BF16/TF32
- Weak for modern LLMs
notable_users:
- Google Colab (free tier)
- AWS g4dn
- Budget inference services
image: /images/gpus/nvidia-t4.jpg
tags:
- nvidia
- datacenter
- turing
updated: '2026-11-21'
sources:
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

Budget-friendly inference GPU. Still widely deployed but increasingly dated for modern LLM workloads.
