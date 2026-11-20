---
id: gpu/nvidia-a100-40gb
type: gpu
slug: nvidia-a100-40gb
schema_version: 1.1
title: A100 40GB
vendor: NVIDIA
segment: datacenter
series: Ampere
generation: Ampere
release_date: '2020-06-22'
signal_strength: medium
summary: Original A100 variant. Still widely used for smaller model training and inference workloads.
aliases:
- NVIDIA A100 40GB
specifications:
  memory_gb: 40
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 1555
  unit_kind: gpu
  compute_units: 6912
  compute_unit_type: CUDA Cores
  tensor_cores: 432
  tdp_watts: 400
  form_factor:
  - SXM4
  pcie_gen: 4.0
  interconnect:
    name: NVLink 3.0
    bandwidth_gb_per_s: 600
  process_node:
    nodes_nm:
    - 7
performance:
  fp32_tflops: 19.5
  fp16_tflops: 312.0
  bf16_tflops: 312.0
  tf32_tflops: 156.0
  int8_tops: 624.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 20
  max_model_params_b_training: 7
  sparsity_support: true
  transformer_engine: false
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
  msrp_usd: 10000
  cloud_hourly_usd: 1.1
  cloud_providers:
  - name: Various CSPs
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Training smaller models
- Inference for 7B-13B models
- Cost-effective multi-GPU setups
key_features:
- 40 GB HBM2e
- Multi-Instance GPU (MIG)
- 3rd-gen Tensor Cores
- Structural sparsity (2:4)
limitations:
- 40GB limits large model loading
- No FP8 support
- Lower memory bandwidth
notable_users:
- Cloud providers
- Universities
- Research labs
image: /images/gpus/nvidia-a100-40gb.jpg
tags:
- nvidia
- datacenter
- ampere
updated: '2026-11-20'
sources:
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/a100/pdf/nvidia-a100-datasheet-us-nvidia-1758950-r4-web.pdf
  title: NVIDIA A100 Tensor Core GPU data sheet (NVIDIA)
- url: https://www.nvidia.com/en-us/data-center/a100/
  title: NVIDIA A100 Tensor Core GPU (NVIDIA)
---

## Overview

Original A100 variant. Still widely used for smaller model training and inference workloads.
