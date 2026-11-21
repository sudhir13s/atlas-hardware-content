---
id: gpu/nvidia-a6000
type: gpu
slug: nvidia-a6000
schema_version: 1.4
title: RTX A6000
vendor: NVIDIA
segment: workstation
series: Ampere
generation: Ampere
signal_strength: medium
summary: NVIDIA workstation GPU on the Ampere architecture with 48 GB of GDDR6 with ECC at 768 GB/s, and NVLink to connect two cards.
aliases:
- NVIDIA RTX A6000
specifications:
  memory_gb: 48
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 768
  unit_kind: gpu
  compute_units: 10752
  compute_unit_type: CUDA Cores
  tensor_cores: 336
  rt_cores: 84
  tdp_watts: 300
  form_factor:
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: NVLink
    bandwidth_gb_per_s: 112.5
    note: bidirectional
  process_node:
    nodes_nm:
    - 8
    note: Samsung 8 nm 8N NVIDIA Custom Process
performance:
  fp32_tflops: 38.7
  fp16_tflops: 154.8
  bf16_tflops: 154.8
  tf32_tflops: 77.4
  int8_tops: 309.7
  basis: dense
  performance_basis_note: Dense peaks at GPU Boost Clock from NVIDIA's GA102 whitepaper; fp16 and bf16 are Tensor TFLOPS with FP32 accumulate; with sparsity NVIDIA lists twice the Tensor figures (the datasheet's 'Tensor performance 309.7 TFLOPS' is with sparsity).
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: NVLink
    max_units: 2
    note: combined graphics memory of up to 96 GB
framework_support:
  pytorch: true
  tensorflow: true
  jax: true
  onnx_runtime: true
  tensorrt: true
  directml: true
  mlx: false
  rocm: false
  oneapi: false
  triton: true
  vllm: true
  deepspeed: true
market:
  cloud_hourly_usd: 0.57
  observed_at: '2026-11-20'
  source: Epoch AI machine learning hardware; GetDeploying GPU cloud prices
best_for:
- Rendering
- AI
- Graphics
- Compute
key_features:
- 48 GB GDDR6 with ECC
- NVLink, 112.5 GB/s bidirectional, two GPUs
- 300 W total board power
- Dual-slot PCIe 4.0 x16 card
notable_users:
- South Park (studio)
image: /images/gpus/nvidia-a6000.jpg
tags:
- nvidia
- workstation
- ampere
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/design-visualization/quadro-product-literature/proviz-print-nvidia-rtx-a6000-datasheet-us-nvidia-1454980-r9-web%20(1).pdf
  title: NVIDIA RTX A6000 Datasheet (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/content/PDF/nvidia-ampere-ga-102-gpu-architecture-whitepaper-v2.pdf
  title: NVIDIA Ampere GA102 GPU Architecture Whitepaper (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-brings-millions-more-into-the-metaverse-with-expanded-omniverse-platform
  title: NVIDIA Brings Millions More Into the Metaverse With Expanded Omniverse Platform (NVIDIA Newsroom, August 10, 2021)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

NVIDIA workstation GPU on the Ampere architecture with 48 GB of GDDR6 with ECC at 768 GB/s, and NVLink to connect two cards.
