---
id: gpu/nvidia-b200
type: gpu
slug: nvidia-b200
schema_version: 1.4
title: B200
vendor: NVIDIA
segment: datacenter
series: Blackwell
generation: Blackwell
release_date: '2024-03-18'
signal_strength: high
summary: NVIDIA datacenter GPU on the Blackwell architecture with 180 GB of HBM3e at up to 8 TB/s in the SXM form factor.
aliases:
- NVIDIA B200
specifications:
  memory_gb: 180
  memory_type: HBM3e
  memory_bandwidth_gb_per_s: 8000
  unit_kind: gpu
  tdp_watts: 1000
  form_factor:
  - SXM
  pcie_gen: 5.0
  interconnect:
    name: Fifth-generation NVLink
    bandwidth_gb_per_s: 1800
    note: bidirectional per GPU
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4NP
performance: {}
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: Fifth-generation NVLink and fourth-generation NVSwitch (HGX B200)
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
  cloud_hourly_usd: 8.12
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
key_features:
- Two dies joined by a 10 TB/s chip-to-chip link into one GPU
- 180 GB HBM3e, up to 8 TB/s
- Fifth-generation NVLink, 1.8 TB/s
- Configurable up to 1 kW per GPU
image: /images/gpus/nvidia-b200.jpg
tags:
- nvidia
- datacenter
- blackwell
updated: '2026-11-21'
sources:
- url: https://docs.nvidia.com/enterprise-reference-architectures/hgx-ai-factory-h100-h200-b200/latest/components.html
  title: NVIDIA HGX AI Factory (HGX H100, H200, B200) Components (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-blackwell-platform-arrives-to-power-a-new-era-of-computing
  title: NVIDIA Blackwell Platform Arrives to Power a New Era of Computing (NVIDIA Newsroom)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/hgx/
  title: NVIDIA HGX Platform (NVIDIA)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

NVIDIA datacenter GPU on the Blackwell architecture with 180 GB of HBM3e at up to 8 TB/s in the SXM form factor.
