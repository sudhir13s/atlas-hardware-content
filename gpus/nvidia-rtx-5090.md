---
id: gpu/nvidia-rtx-5090
type: gpu
slug: nvidia-rtx-5090
schema_version: 3.0
title: GeForce RTX 5090
vendor: NVIDIA
segment: consumer
series: GeForce RTX 50
generation: Blackwell
architecture: gpu-architecture/blackwell
compute_platform: cuda
compute_capability: 12.0
release_date: '2025-01-30'
signal_strength: medium
summary: NVIDIA consumer GPU on the Blackwell architecture with 32 GB of GDDR7 at 1792 GB/s.
aliases:
- NVIDIA GeForce RTX 5090
specifications:
  memory_gb: 32
  memory_type: GDDR7
  memory_bandwidth_gb_per_s: 1792
  unit_kind: gpu
  compute_units: 21760
  compute_unit_type: CUDA Cores
  tensor_cores: 680
  rt_cores: 170
  tdp_watts: 575
  form_factor:
  - PCIe
  pcie_gen: 5.0
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4nm 4N NVIDIA Custom Process
performance:
  fp32_tflops: 104.8
  fp16_tflops: 209.5
  bf16_tflops: 209.5
  tf32_tflops: 104.8
  fp8_tflops: 419
  int8_tops: 838
  basis: dense
  performance_basis_note: Dense peaks at GPU Boost Clock from NVIDIA's RTX Blackwell whitepaper; fp16, bf16 and fp8 are Tensor TFLOPS with FP32 accumulate (with FP16 accumulate NVIDIA lists FP16 419 and FP8 838); with sparsity NVIDIA lists twice the Tensor figures.
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
market:
  msrp_usd: 1999
  msrp_source: https://nvidianews.nvidia.com/news/nvidia-blackwell-geforce-rtx-50-series-opens-new-world-of-ai-computer-graphics
  msrp_announced: '2025-01-06'
  cloud_hourly_usd: 0.72
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- AI models
- Creative workloads
- Gaming
key_features:
- 32 GB GDDR7, 512-bit
- Fifth-generation Tensor Cores with FP4
- 575 W total graphics power
- PCIe Gen 5
- DLSS 4 with Multi Frame Generation
limitations:
- No NVLink
image: /images/gpus/nvidia-rtx-5090.jpg
tags:
- nvidia
- consumer
- blackwell
updated: '2026-11-24'
sources:
- url: https://images.nvidia.com/aem-dam/Solutions/geforce/blackwell/nvidia-rtx-blackwell-gpu-architecture.pdf
  title: NVIDIA RTX Blackwell GPU Architecture Whitepaper (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5090/
  title: GeForce RTX 5090 (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-blackwell-geforce-rtx-50-series-opens-new-world-of-ai-computer-graphics
  title: NVIDIA Blackwell GeForce RTX 50 Series Opens New World of AI Computer Graphics (NVIDIA Newsroom, January 6, 2025)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---


