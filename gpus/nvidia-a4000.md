---
id: gpu/nvidia-a4000
type: gpu
slug: nvidia-a4000
schema_version: 2.0
title: RTX A4000
vendor: NVIDIA
segment: workstation
series: Ampere
generation: Ampere
compute_platform: cuda
compute_capability: 8.6
release_date: '2021-04-12'
signal_strength: low
summary: NVIDIA workstation GPU on the Ampere architecture with 16 GB of GDDR6 with ECC at 448 GB/s in a single-slot PCIe card.
aliases:
- NVIDIA RTX A4000
specifications:
  memory_gb: 16
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 448
  unit_kind: gpu
  compute_units: 6144
  compute_unit_type: CUDA Cores
  tensor_cores: 192
  rt_cores: 48
  tdp_watts: 140
  form_factor:
  - PCIe (single-slot)
  pcie_gen: 4.0
performance:
  fp32_tflops: 19.2
  performance_basis_note: NVIDIA lists single-precision peak at GPU Boost Clock; its only Tensor figure (153.4 TFLOPS) is with sparsity and names no precision.
ml_capabilities:
  inference: true
  training: false
  fine_tuning: true
  sparsity_support: true
  transformer_engine: false
market:
  cloud_hourly_usd: 0.25
  observed_at: '2026-11-20'
  source: Epoch AI machine learning hardware; GetDeploying GPU cloud prices
best_for:
- Real-time ray tracing
- AI-accelerated compute
- Graphics
key_features:
- 16 GB GDDR6 with ECC
- Single-slot PCIe card
- 140 W total board power
- PCIe 4.0 x16
image: /images/gpus/nvidia-a4000.jpg
tags:
- nvidia
- workstation
- ampere
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/gtcs21/rtx-a4000/nvidia-rtx-a4000-datasheet.pdf
  title: NVIDIA RTX A4000 Datasheet (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/new-nvidia-rtx-gpus-power-next-generation-of-workstations-and-pcs-for-millions-of-artists-designers-engineers-and-virtual-desktop-users
  title: New NVIDIA RTX GPUs Power Next Generation of Workstations and PCs (NVIDIA Newsroom, April 12, 2021)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---

## Overview

NVIDIA workstation GPU on the Ampere architecture with 16 GB of GDDR6 with ECC at 448 GB/s in a single-slot PCIe card.
