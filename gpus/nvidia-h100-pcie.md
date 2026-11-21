---
id: gpu/nvidia-h100-pcie
type: gpu
slug: nvidia-h100-pcie
schema_version: 1.4
title: H100 PCIe
vendor: NVIDIA
segment: datacenter
series: Hopper
generation: Hopper
release_date: '2022-03-22'
signal_strength: high
summary: NVIDIA datacenter GPU on the Hopper architecture with 80 GB of HBM2e at 2,000 GB/s on a dual-slot, passively cooled PCIe Gen5 card.
aliases:
- NVIDIA H100 PCIe
specifications:
  memory_gb: 80
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 2000
  unit_kind: gpu
  compute_units: 14592
  compute_unit_type: CUDA Cores
  tensor_cores: 456
  tdp_watts: 350
  form_factor:
  - PCIe
  pcie_gen: 5.0
  interconnect:
    name: NVLink bridge
    bandwidth_gb_per_s: 600
    note: total, between two bridged H100 PCIe cards
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4N
performance: {}
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: NVLink bridge (one adjacent H100 PCIe card)
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
  cloud_hourly_usd: 2.5
  cloud_providers:
  - name: Various CSPs
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- AI
- Data analytics
- High-performance computing
key_features:
- 80 GB HBM2e, 2,000 GB/s
- PCI Express Gen5 x16
- 350 W maximum board power
- Passive heat sink, dual-slot full-height full-length card
- Multi-Instance GPU (up to seven instances)
image: /images/gpus/nvidia-h100-pcie.jpg
tags:
- nvidia
- datacenter
- hopper
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/gtcs22/data-center/h100/PB-11133-001_v01.pdf
  title: NVIDIA H100 PCIe GPU Product Brief (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/
  title: NVIDIA Hopper Architecture In-Depth (NVIDIA Technical Blog)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-announces-hopper-architecture-the-next-generation-of-accelerated-computing
  title: NVIDIA Announces Hopper Architecture, the Next Generation of Accelerated Computing (NVIDIA Newsroom, March 22, 2022)
  trust: 0.95
---

## Overview

NVIDIA datacenter GPU on the Hopper architecture with 80 GB of HBM2e at 2,000 GB/s on a dual-slot, passively cooled PCIe Gen5 card.
