---
id: gpu/nvidia-rtx-4080
type: gpu
slug: nvidia-rtx-4080
schema_version: 3.0
title: GeForce RTX 4080
vendor: NVIDIA
segment: consumer
series: GeForce RTX 40
generation: Ada Lovelace
architecture: gpu-architecture/ada-lovelace
compute_platform: cuda
compute_capability: 8.9
release_date: '2022-11-16'
signal_strength: low
summary: NVIDIA consumer GPU on the Ada Lovelace architecture with 16 GB of GDDR6X at 716.8 GB/s.
aliases:
- NVIDIA GeForce RTX 4080
specifications:
  memory_gb: 16
  memory_type: GDDR6X
  memory_bandwidth_gb_per_s: 716.8
  unit_kind: gpu
  compute_units: 9728
  compute_unit_type: CUDA Cores
  tensor_cores: 304
  rt_cores: 76
  tdp_watts: 320
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4N NVIDIA Custom Process
performance:
  fp32_tflops: 48.7
  fp16_tflops: 97.5
  bf16_tflops: 97.5
  tf32_tflops: 48.7
  fp8_tflops: 194.9
  int8_tops: 389.9
  basis: dense
  performance_basis_note: Dense peaks at GPU Boost Clock for the RTX 4080 16 GB from NVIDIA's Ada whitepaper; fp16, bf16 and fp8 are Tensor TFLOPS with FP32 accumulate (with FP16 accumulate NVIDIA lists FP16 194.9 and FP8 389.9); with sparsity NVIDIA lists twice the Tensor figures.
ml_capabilities:
  inference: true
  training: false
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
market:
  msrp_usd: 1199
  msrp_source: https://nvidianews.nvidia.com/news/nvidia-delivers-quantum-leap-in-performance-introduces-new-era-of-neural-rendering-with-geforce-rtx-40-series
  msrp_announced: '2022-09-20'
  cloud_hourly_usd: 0.304
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Gaming
- Content creation
key_features:
- 16 GB GDDR6X, 256-bit
- Fourth-generation Tensor Cores with FP8
- 320 W total graphics power
- PCIe Gen 4
limitations:
- No NVLink
image: /images/gpus/nvidia-rtx-4080.jpg
tags:
- nvidia
- consumer
- ada-lovelace
updated: '2026-11-24'
sources:
- url: https://images.nvidia.com/aem-dam/Solutions/geforce/ada/nvidia-ada-gpu-architecture.pdf
  title: NVIDIA Ada GPU Architecture Whitepaper (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4080-family/
  title: GeForce RTX 4080 Family (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/news/geforce-rtx-4080-out-now
  title: 'GeForce RTX 4080 Out Now: Beyond Fast For Gamers & Creators (NVIDIA GeForce News, November 16, 2022)'
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---


