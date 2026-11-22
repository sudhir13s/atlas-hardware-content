---
id: gpu/nvidia-rtx-3080
type: gpu
slug: nvidia-rtx-3080
schema_version: 2.0
title: GeForce RTX 3080
vendor: NVIDIA
segment: consumer
series: GeForce RTX 30
generation: Ampere
compute_platform: cuda
compute_capability: 8.6
release_date: '2020-09-17'
signal_strength: low
summary: NVIDIA consumer GPU on the Ampere architecture with 10 GB of GDDR6X at 760 GB/s.
aliases:
- NVIDIA GeForce RTX 3080
specifications:
  memory_gb: 10
  memory_type: GDDR6X
  memory_bandwidth_gb_per_s: 760
  unit_kind: gpu
  compute_units: 8704
  compute_unit_type: CUDA Cores
  tensor_cores: 272
  rt_cores: 68
  tdp_watts: 320
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 8
    note: Samsung 8 nm 8N NVIDIA Custom Process
performance:
  fp32_tflops: 29.8
  fp16_tflops: 59.5
  bf16_tflops: 59.5
  tf32_tflops: 29.8
  int8_tops: 238
  basis: dense
  performance_basis_note: Dense peaks at GPU Boost Clock for the RTX 3080 10 GB Founders Edition from NVIDIA's GA102 whitepaper; fp16 and bf16 are Tensor TFLOPS with FP32 accumulate (FP16 accumulate 119); with sparsity NVIDIA lists twice the Tensor figures.
ml_capabilities:
  inference: true
  training: false
  fine_tuning: false
  sparsity_support: true
  transformer_engine: false
market:
  msrp_usd: 699
  msrp_source: https://nvidianews.nvidia.com/news/nvidia-delivers-greatest-ever-generational-leap-in-performance-with-geforce-rtx-30-series-gpus
  msrp_announced: '2020-09-01'
  cloud_hourly_usd: 0.14
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- 4K gaming
key_features:
- 10 GB GDDR6X, 320-bit
- 320 W graphics card power
- PCIe Gen 4
limitations:
- No NVLink
- No FP8 Tensor Core support
image: /images/gpus/nvidia-rtx-3080.jpg
tags:
- nvidia
- consumer
- ampere
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/content/PDF/nvidia-ampere-ga-102-gpu-architecture-whitepaper-v2.pdf
  title: NVIDIA Ampere GA102 GPU Architecture Whitepaper (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/30-series/rtx-3080-3080ti/
  title: GeForce RTX 3080 Family (NVIDIA)
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

NVIDIA consumer GPU on the Ampere architecture with 10 GB of GDDR6X at 760 GB/s.
