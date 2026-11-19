---
id: gpu/nvidia-v100-16gb
type: gpu
slug: nvidia-v100-16gb
schema_version: 1.1
title: V100 16GB
vendor: NVIDIA
segment: datacenter
series: Volta
generation: Volta
release_date: '2017-06-21'
signal_strength: low
summary: Original V100 with 16GB. Largely retired from production but still available on older cloud instances.
aliases:
- NVIDIA V100 16GB
specifications:
  memory_gb: 16
  memory_type: HBM2
  memory_bandwidth_gb_per_s: 900
  unit_kind: gpu
  compute_units: 5120
  compute_unit_type: CUDA Cores
  tensor_cores: 640
  tdp_watts: 300
  form_factor:
  - SXM2
  - PCIe
  pcie_gen: 3.0
  interconnect:
    name: NVLink 2.0
    bandwidth_gb_per_s: 300
  process_node:
    nodes_nm:
    - 12
performance:
  fp32_tflops: 15.7
  fp16_tflops: 125.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 7
  max_model_params_b_training: 2
  sparsity_support: false
  transformer_engine: false
  multi_gpu_scaling:
    technology: NVLink 2.0
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
  vllm: false
  deepspeed: true
market:
  msrp_usd: 6000
  cloud_hourly_usd: 0.7
  cloud_providers:
  - name: AWS
    instance_note: p3
  - name: GCP
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Legacy workloads
- Small model training
- Educational use
key_features:
- 16 GB HBM2
- First generation Tensor Cores
- Good for smaller models
limitations:
- 16GB very limiting for modern models
- No BF16/TF32/FP8
- End of life
notable_users:
- Universities
- Legacy cloud instances
image: /images/gpus/nvidia-v100-16gb.jpg
tags:
- nvidia
- datacenter
- volta
updated: '2026-11-19'
sources: []
---

## Overview

Original V100 with 16GB. Largely retired from production but still available on older cloud instances.
