---
id: gpu/nvidia-rtx-4090
type: gpu
slug: nvidia-rtx-4090
schema_version: 3.0
title: GeForce RTX 4090
vendor: NVIDIA
segment: consumer
series: GeForce RTX 40
generation: Ada Lovelace
architecture: gpu-architecture/ada-lovelace
compute_platform: cuda
compute_capability: 8.9
release_date: '2022-10-12'
signal_strength: medium
summary: NVIDIA consumer GPU on the Ada Lovelace architecture with 24 GB of GDDR6X at 1008 GB/s.
aliases:
- NVIDIA GeForce RTX 4090
specifications:
  memory_gb: 24
  memory_type: GDDR6X
  memory_bandwidth_gb_per_s: 1008
  unit_kind: gpu
  compute_units: 16384
  compute_unit_type: CUDA Cores
  tensor_cores: 512
  rt_cores: 128
  tdp_watts: 450
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4N NVIDIA Custom Process
performance:
  fp32_tflops: 82.6
  fp16_tflops: 165.2
  bf16_tflops: 165.2
  tf32_tflops: 82.6
  fp8_tflops: 330.3
  int8_tops: 660.6
  basis: dense
  performance_basis_note: Dense peaks at GPU Boost Clock from NVIDIA's Ada whitepaper; fp16, bf16 and fp8 are Tensor TFLOPS with FP32 accumulate (with FP16 accumulate NVIDIA lists FP16 330.3 and FP8 660.6); with sparsity NVIDIA lists twice the Tensor figures.
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
market:
  msrp_usd: 1599
  msrp_source: https://nvidianews.nvidia.com/news/nvidia-delivers-quantum-leap-in-performance-introduces-new-era-of-neural-rendering-with-geforce-rtx-40-series
  msrp_announced: '2022-09-20'
  cloud_hourly_usd: 0.456
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Gaming
- Content creation
key_features:
- 24 GB GDDR6X, 384-bit
- Fourth-generation Tensor Cores with FP8
- 450 W total graphics power
- DLSS 3
limitations:
- No NVLink
image: /images/gpus/nvidia-rtx-4090.jpg
tags:
- nvidia
- consumer
- ada-lovelace
updated: '2026-11-24'
sources:
- url: https://images.nvidia.com/aem-dam/Solutions/geforce/ada/nvidia-ada-gpu-architecture.pdf
  title: NVIDIA Ada GPU Architecture Whitepaper (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/
  title: GeForce RTX 4090 (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-delivers-quantum-leap-in-performance-introduces-new-era-of-neural-rendering-with-geforce-rtx-40-series
  title: NVIDIA Delivers Quantum Leap in Performance, Introduces New Era of Neural Rendering With GeForce RTX 40 Series (NVIDIA Newsroom, September 20, 2022)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---


