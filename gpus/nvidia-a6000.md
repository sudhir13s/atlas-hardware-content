---
id: gpu/nvidia-a6000
type: gpu
slug: nvidia-a6000
schema_version: 1.1
title: RTX A6000
vendor: NVIDIA
segment: workstation
series: Ampere
generation: Ampere
release_date: '2020-12-03'
signal_strength: medium
summary: NVIDIA's professional workstation GPU with 48GB, popular for local ML development and fine-tuning.
aliases:
- NVIDIA RTX A6000
specifications:
  memory_gb: 48
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 768
  unit_kind: gpu
  compute_units: 10752
  compute_unit_type: CUDA Cores
  tensor_cores: 336
  rt_cores: 84
  tdp_watts: 300
  form_factor:
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: NVLink
    bandwidth_gb_per_s: 112.5
  process_node:
    nodes_nm:
    - 8
performance:
  fp32_tflops: 38.7
  fp16_tflops: 77.4
  bf16_tflops: 77.4
  tf32_tflops: 77.4
  int8_tops: 309.7
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 25
  max_model_params_b_training: 10
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
  cloud_hourly_usd: 0.57
  observed_at: '2026-11-20'
  source: Epoch AI machine learning hardware; GetDeploying GPU cloud prices
best_for:
- Workstation ML development
- Local fine-tuning
- Data science
- 3D + AI workflows
key_features:
- 48 GB GDDR6
- NVLink bridge for 2-GPU
- ECC memory
- Professional driver support
limitations:
- GDDR6 has lower bandwidth than HBM
- Workstation pricing
- Single slot requires good airflow
notable_users:
- ML engineers
- Data science teams
- VFX studios
image: /images/gpus/nvidia-a6000.jpg
tags:
- nvidia
- workstation
- ampere
updated: '2026-11-21'
sources:
- url: https://epoch.ai/data/ml_hardware.csv
  title: Epoch AI, "Data on Machine Learning Hardware" (epoch.ai/data/machine-learning-hardware), CC BY; credit Epoch AI as the source.
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

NVIDIA's professional workstation GPU with 48GB, popular for local ML development and fine-tuning.
