---
id: gpu/nvidia-h100-sxm
type: gpu
slug: nvidia-h100-sxm
schema_version: 2.0
title: H100 SXM
vendor: NVIDIA
segment: datacenter
series: Hopper
generation: Hopper
compute_platform: cuda
compute_capability: 9.0
release_date: '2022-09-20'
signal_strength: high
summary: NVIDIA datacenter GPU on the Hopper architecture with 80 GB of HBM3 at 3.35 TB/s in the SXM5 form factor.
aliases:
- NVIDIA H100 SXM
specifications:
  memory_gb: 80
  memory_type: HBM3
  memory_bandwidth_gb_per_s: 3350
  unit_kind: gpu
  compute_units: 16896
  compute_unit_type: CUDA Cores
  tensor_cores: 528
  tdp_watts: 700
  form_factor:
  - SXM5
  interconnect:
    name: Fourth-generation NVLink
    bandwidth_gb_per_s: 900
    note: bidirectional per GPU
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4N
performance:
  fp32_tflops: 67.0
  fp16_tflops: 1979.0
  bf16_tflops: 1979.0
  tf32_tflops: 989.0
  fp8_tflops: 3958.0
  int8_tops: 3958.0
  basis: sparse
  performance_basis_note: NVIDIA lists the Tensor Core figures (TF32, BF16, FP16, FP8, INT8) with sparsity; FP32 is a non-Tensor Core figure.
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: Fourth-generation NVLink and third-generation NVSwitch (HGX H100)
market:
  cloud_hourly_usd: 3.5
  cloud_providers:
  - name: AWS
    instance_note: p5 instances
  observed_at: '2026-06-15'
  source: snapshot
key_features:
- 80 GB HBM3, 3.35 TB/s
- Transformer Engine with FP8
- Fourth-generation NVLink, 900 GB/s
- Confidential Computing
notable_users:
- Amazon Web Services
- Google Cloud
- Microsoft Azure
- Oracle Cloud Infrastructure
image: /images/gpus/nvidia-h100-sxm.jpg
tags:
- nvidia
- datacenter
- hopper
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 GPU (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/
  title: NVIDIA Hopper Architecture In-Depth (NVIDIA Technical Blog)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-hopper-in-full-production
  title: NVIDIA Hopper in Full Production (NVIDIA Newsroom)
  trust: 0.95
- url: https://docs.nvidia.com/enterprise-reference-architectures/hgx-ai-factory-h100-h200-b200/latest/components.html
  title: NVIDIA HGX AI Factory (HGX H100, H200, B200) Components (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/technologies/hopper-architecture/
  title: NVIDIA Hopper Architecture (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---

## Overview

NVIDIA datacenter GPU on the Hopper architecture with 80 GB of HBM3 at 3.35 TB/s in the SXM5 form factor.
