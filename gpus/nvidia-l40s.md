---
id: gpu/nvidia-l40s
type: gpu
slug: nvidia-l40s
schema_version: 2.0
title: L40S
vendor: NVIDIA
segment: datacenter
series: Ada Lovelace
generation: Ada Lovelace
compute_platform: cuda
compute_capability: 8.9
release_date: '2023-08-08'
signal_strength: medium
summary: NVIDIA datacenter GPU on the Ada Lovelace architecture with 48 GB of GDDR6 with ECC at 864 GB/s in a 350 W dual-slot PCIe card.
aliases:
- NVIDIA L40S
specifications:
  memory_gb: 48
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 864
  unit_kind: gpu
  compute_units: 18176
  compute_unit_type: CUDA Cores
  tensor_cores: 568
  rt_cores: 142
  tdp_watts: 350
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4N
performance:
  fp32_tflops: 91.6
  fp16_tflops: 362.05
  bf16_tflops: 362.05
  tf32_tflops: 183.0
  fp8_tflops: 733.0
  int8_tops: 733.0
  basis: dense
  performance_basis_note: dense; with sparsity NVIDIA lists TF32 366, FP16/BF16 733, FP8 1,466 TFLOPS and INT8 1,466 TOPS
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
market:
  cloud_hourly_usd: 1.8
  cloud_providers:
  - name: AWS
    instance_note: g6e
  - name: GCP
  - name: Azure
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Generative AI
- LLM training and inference
- Rendering and 3D graphics
- Video processing
- NVIDIA Omniverse
key_features:
- 48 GB GDDR6 with ECC, 864 GB/s
- Fourth-generation Tensor Cores with FP8 Transformer Engine
- 142 third-generation RT Cores
- 3 NVENC and 3 NVDEC engines with AV1 encode and decode
limitations:
- No NVLink support
- No MIG support
notable_users:
- CoreWeave
image: /images/gpus/nvidia-l40s.jpg
tags:
- nvidia
- datacenter
- ada-lovelace
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/en-us/data-center/l40s/
  title: NVIDIA L40S GPU (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-global-data-center-system-manufacturers-to-supercharge-generative-ai-and-industrial-digitalization
  title: NVIDIA, Global Data Center System Manufacturers to Supercharge Generative AI and Industrial Digitalization (L40S announcement, NVIDIA Newsroom)
  trust: 0.95
- url: https://images.nvidia.com/aem-dam/Solutions/geforce/ada/nvidia-ada-gpu-architecture.pdf
  title: NVIDIA Ada GPU Architecture whitepaper (NVIDIA)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---

## Overview

NVIDIA datacenter GPU on the Ada Lovelace architecture with 48 GB of GDDR6 with ECC at 864 GB/s in a 350 W dual-slot PCIe card.
