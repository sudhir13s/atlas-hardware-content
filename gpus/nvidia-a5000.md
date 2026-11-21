---
id: gpu/nvidia-a5000
type: gpu
slug: nvidia-a5000
schema_version: 1.1
title: RTX A5000
vendor: NVIDIA
segment: workstation
series: Ampere
generation: Ampere
release_date: '2021-04-12'
signal_strength: low
summary: Mid-range professional GPU with 24GB VRAM for ML development workstations.
aliases:
- NVIDIA RTX A5000
specifications:
  memory_gb: 24
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 768
  unit_kind: gpu
  compute_units: 8192
  compute_unit_type: CUDA Cores
  tensor_cores: 256
  rt_cores: 64
  tdp_watts: 230
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
  fp32_tflops: 27.8
  fp16_tflops: 55.6
  bf16_tflops: 55.6
  tf32_tflops: 55.6
  int8_tops: 222.2
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 13
  max_model_params_b_training: 5
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
  cloud_hourly_usd: 1.3403
  observed_at: '2026-11-20'
  source: Epoch AI machine learning hardware; GetDeploying GPU cloud prices
best_for:
- Workstation ML development
- Fine-tuning smaller models
- Data science
key_features:
- 24 GB GDDR6 with ECC
- NVLink bridge support
- Professional drivers
- Good balance of price and VRAM
limitations:
- 24GB VRAM limits larger models
- Lower compute than A6000
notable_users:
- Enterprise data science teams
- Academic researchers
image: /images/gpus/nvidia-a5000.jpg
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

Mid-range professional GPU with 24GB VRAM for ML development workstations.
