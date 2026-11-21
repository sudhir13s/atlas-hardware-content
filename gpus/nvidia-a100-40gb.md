---
id: gpu/nvidia-a100-40gb
type: gpu
slug: nvidia-a100-40gb
schema_version: 1.4
title: A100 40GB
vendor: NVIDIA
segment: datacenter
series: Ampere
generation: Ampere
release_date: '2020-05-14'
signal_strength: medium
summary: NVIDIA datacenter GPU on the Ampere architecture with 40 GB of HBM2 at 1,555 GB/s in the SXM form factor.
aliases:
- NVIDIA A100 40GB
specifications:
  memory_gb: 40
  memory_type: HBM2
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
    name: Third-generation NVLink
    bandwidth_gb_per_s: 600
  process_node:
    nodes_nm:
    - 7
    note: TSMC 7nm N7
performance:
  fp32_tflops: 19.5
  fp16_tflops: 312.0
  bf16_tflops: 312.0
  tf32_tflops: 156.0
  int8_tops: 624.0
  basis: dense
  performance_basis_note: dense; with sparsity NVIDIA lists twice these Tensor Core figures (TF32 312, FP16/BF16 624 TFLOPS, INT8 1,248 TOPS)
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: NVLink and NVSwitch
    max_units: 16
    note: up to 16 A100 GPUs at up to 600 GB/s
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
  cloud_hourly_usd: 1.1
  cloud_providers:
  - name: Various CSPs
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- AI training
- AI inference
- Data analytics
- High-performance computing (HPC)
key_features:
- 40 GB HBM2, 1,555 GB/s
- Multi-Instance GPU (MIG), up to 7 instances of 5 GB
- Third-generation Tensor Cores
- Structural sparsity
- Third-generation NVLink, 600 GB/s
notable_users:
- Microsoft (Azure)
image: /images/gpus/nvidia-a100-40gb.jpg
tags:
- nvidia
- datacenter
- ampere
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/a100/pdf/nvidia-a100-datasheet-us-nvidia-1758950-r4-web.pdf
  title: NVIDIA A100 Tensor Core GPU data sheet (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/blog/nvidia-ampere-architecture-in-depth/
  title: NVIDIA Ampere Architecture In-Depth (NVIDIA Technical Blog)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidias-new-ampere-data-center-gpu-in-full-production
  title: NVIDIA's New Ampere Data Center GPU in Full Production (NVIDIA Newsroom)
  trust: 0.95
---

## Overview

NVIDIA datacenter GPU on the Ampere architecture with 40 GB of HBM2 at 1,555 GB/s in the SXM form factor.
