---
id: gpu/nvidia-gb300
type: gpu
slug: nvidia-gb300
schema_version: 2.0
title: GB300 Grace Blackwell Ultra Superchip
vendor: NVIDIA
segment: datacenter
series: Blackwell Ultra
generation: Blackwell Ultra
compute_platform: cuda
compute_capability: 10.3
release_date: '2025-03-18'
signal_strength: high
summary: NVIDIA superchip that joins two Blackwell Ultra GPUs, each with 288 GB of HBM3e at 8 TB/s, to one Grace CPU.
aliases:
- NVIDIA GB300 Grace Blackwell Ultra Superchip
specifications:
  memory_type: HBM3e
  memory_note: 288 GB HBM3e at 8 TB/s per Blackwell Ultra GPU
  unit_kind: module
  gpus_per_module: 2
  form_factor:
  - Superchip Module
  interconnect:
    name: Fifth-generation NVLink
    bandwidth_gb_per_s: 1800
    note: bidirectional per GPU
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4NP (Blackwell Ultra GPUs)
performance: {}
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: Fifth-generation NVLink (GB300 NVL72, 72 GPUs)
market:
  cloud_hourly_usd: 18.0
  observed_at: '2026-11-20'
  source: GetDeploying GPU cloud prices
key_features:
- 1 Grace CPU and 2 Blackwell Ultra GPUs
- 900 GB/s NVLink-C2C link between CPU and GPUs
- 288 GB HBM3e per GPU
- Building block of the GB300 NVL72 rack (72 GPUs, 36 Grace CPUs)
image: /images/gpus/nvidia-gb300.jpg
tags:
- nvidia
- datacenter
- blackwell-ultra
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/en-us/data-center/gb300-nvl72/
  title: NVIDIA GB300 NVL72 (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/blog/inside-nvidia-blackwell-ultra-the-chip-powering-the-ai-factory-era/
  title: 'Inside NVIDIA Blackwell Ultra: The Chip Powering the AI Factory Era (NVIDIA Technical Blog)'
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-blackwell-ultra-ai-factory-platform-paves-way-for-age-of-ai-reasoning
  title: NVIDIA Blackwell Ultra AI Factory Platform Paves Way for Age of AI Reasoning (NVIDIA Newsroom)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---

## Overview

NVIDIA superchip that joins two Blackwell Ultra GPUs, each with 288 GB of HBM3e at 8 TB/s, to one Grace CPU.
