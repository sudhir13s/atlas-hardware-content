---
id: gpu/nvidia-gb200
type: gpu
slug: nvidia-gb200
schema_version: 2.0
title: GB200 Grace Blackwell Superchip
vendor: NVIDIA
segment: datacenter
series: Blackwell
generation: Blackwell
compute_platform: cuda
compute_capability: 10.0
release_date: '2024-03-18'
signal_strength: high
summary: NVIDIA superchip that joins two Blackwell GPUs with 372 GB of HBM3e at 16 TB/s to one 72-core Grace CPU.
aliases:
- NVIDIA GB200 Grace Blackwell Superchip
specifications:
  memory_gb: 372
  memory_type: HBM3e
  memory_note: GPU memory; the Grace CPU adds up to 480 GB LPDDR5X at up to 512 GB/s
  memory_bandwidth_gb_per_s: 16000
  unit_kind: module
  gpus_per_module: 2
  form_factor:
  - Superchip Module
  interconnect:
    name: Fifth-generation NVLink
    bandwidth_gb_per_s: 3600
    note: per superchip
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4NP (Blackwell GPUs)
performance:
  fp32_tflops: 160.0
  fp16_tflops: 10000.0
  bf16_tflops: 10000.0
  tf32_tflops: 5000.0
  fp8_tflops: 20000.0
  int8_tops: 20000.0
  basis: sparse
  performance_basis_note: per superchip; NVIDIA lists the Tensor Core figures (TF32, BF16, FP16, FP8, INT8) with sparsity and states dense is one-half; FP32 is a non-Tensor Core figure.
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: Fifth-generation NVLink (GB200 NVL72, 72 GPUs)
market:
  cloud_hourly_usd: 10.5
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
key_features:
- 1 Grace CPU and 2 B200 GPUs
- 900 GB/s NVLink chip-to-chip link between CPU and GPUs
- 372 GB HBM3e, 16 TB/s
- 72 Arm Neoverse V2 CPU cores
- Building block of the liquid-cooled GB200 NVL72 rack (36 superchips)
image: /images/gpus/nvidia-gb200.jpg
tags:
- nvidia
- datacenter
- blackwell
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/en-us/data-center/gb200-nvl72/
  title: NVIDIA GB200 NVL72 (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-blackwell-platform-arrives-to-power-a-new-era-of-computing
  title: NVIDIA Blackwell Platform Arrives to Power a New Era of Computing (NVIDIA Newsroom)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---

## Overview

NVIDIA superchip that joins two Blackwell GPUs with 372 GB of HBM3e at 16 TB/s to one 72-core Grace CPU.
