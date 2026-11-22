---
id: gpu/nvidia-rtx-3090
type: gpu
slug: nvidia-rtx-3090
schema_version: 2.0
title: GeForce RTX 3090
vendor: NVIDIA
segment: consumer
series: GeForce RTX 30
generation: Ampere
compute_platform: cuda
compute_capability: 8.6
release_date: '2020-09-24'
signal_strength: low
summary: NVIDIA consumer GPU on the Ampere architecture with 24 GB of GDDR6X at 936 GB/s, and NVLink (SLI-Ready) for two cards.
aliases:
- NVIDIA GeForce RTX 3090
specifications:
  memory_gb: 24
  memory_type: GDDR6X
  memory_bandwidth_gb_per_s: 936
  unit_kind: gpu
  compute_units: 10496
  compute_unit_type: CUDA Cores
  tensor_cores: 328
  rt_cores: 82
  tdp_watts: 350
  form_factor:
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: NVLink
    note: SLI-Ready
  process_node:
    nodes_nm:
    - 8
    note: Samsung 8 nm 8N NVIDIA Custom Process
performance:
  fp32_tflops: 35.6
  fp16_tflops: 71
  bf16_tflops: 71
  tf32_tflops: 35.6
  int8_tops: 284
  basis: dense
  performance_basis_note: Dense peaks at GPU Boost Clock for the RTX 3090 Founders Edition from NVIDIA's GA102 whitepaper; fp16 and bf16 are Tensor TFLOPS with FP32 accumulate (FP16 accumulate 142); with sparsity NVIDIA lists twice the Tensor figures.
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: NVLink
    max_units: 2
    note: two RTX 3090 GPUs connect for SLI; 3-way and 4-way SLI not supported
market:
  msrp_usd: 1499
  msrp_source: https://nvidianews.nvidia.com/news/nvidia-delivers-greatest-ever-generational-leap-in-performance-with-geforce-rtx-30-series-gpus
  msrp_announced: '2020-09-01'
  cloud_hourly_usd: 0.22
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- 8K gaming
- AI
- Content creation
key_features:
- 24 GB GDDR6X, 384-bit
- NVLink (SLI-Ready) for two GPUs
- 350 W graphics card power
- PCIe Gen 4
limitations:
- No FP8 Tensor Core support
image: /images/gpus/nvidia-rtx-3090.jpg
tags:
- nvidia
- consumer
- ampere
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/content/PDF/nvidia-ampere-ga-102-gpu-architecture-whitepaper-v2.pdf
  title: NVIDIA Ampere GA102 GPU Architecture Whitepaper (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/30-series/rtx-3090-3090ti/
  title: GeForce RTX 3090 Family (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-delivers-greatest-ever-generational-leap-in-performance-with-geforce-rtx-30-series-gpus
  title: NVIDIA Delivers Greatest-Ever Generational Leap in Performance with GeForce RTX 30 Series GPUs (NVIDIA Newsroom, September 1, 2020)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---

## Overview

NVIDIA consumer GPU on the Ampere architecture with 24 GB of GDDR6X at 936 GB/s, and NVLink (SLI-Ready) for two cards.
