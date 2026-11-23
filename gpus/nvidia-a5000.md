---
id: gpu/nvidia-a5000
type: gpu
slug: nvidia-a5000
schema_version: 3.0
title: RTX A5000
vendor: NVIDIA
segment: workstation
generation: Ampere
architecture: gpu-architecture/ampere
compute_platform: cuda
compute_capability: 8.6
release_date: '2021-04-12'
signal_strength: low
summary: NVIDIA workstation GPU on the Ampere architecture with 24 GB of GDDR6 with ECC at 768 GB/s, and NVLink to connect two cards.
aliases:
- NVIDIA RTX A5000
specifications:
  memory_gb: 24
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 768
  unit_kind: gpu
  compute_units: 8192
  compute_unit_type: CUDA Cores
  tensor_cores: 256
  rt_cores: 64
  tdp_watts: 230
  form_factor:
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: NVLink
    bandwidth_gb_per_s: 112.5
    note: bidirectional
performance:
  fp32_tflops: 27.8
  performance_basis_note: NVIDIA lists single-precision peak at GPU Boost Clock; its only Tensor figure (222.2 TFLOPS) is with sparsity and names no precision.
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: NVLink
    max_units: 2
    note: low-profile bridges connect two RTX A5000 GPUs
market:
  cloud_hourly_usd: 1.3403
  observed_at: '2026-11-20'
  source: Epoch AI machine learning hardware; GetDeploying GPU cloud prices
best_for:
- Rendering
- AI
- Graphics
- Compute
key_features:
- 24 GB GDDR6 with ECC
- NVLink, 112.5 GB/s bidirectional, two GPUs
- 230 W total board power
- PCIe 4.0 x16
notable_users:
- Woods Bagot
- Polaris
- Important Looking Pirates
image: /images/gpus/nvidia-a5000.jpg
tags:
- nvidia
- workstation
- ampere
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/products/workstations/nvidia-rtx-a5000-datasheet.pdf
  title: NVIDIA RTX A5000 Datasheet (NVIDIA)
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


