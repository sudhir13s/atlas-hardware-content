---
id: gpu/nvidia-l4
type: gpu
slug: nvidia-l4
schema_version: 1.4
title: L4
vendor: NVIDIA
segment: datacenter
series: Ada Lovelace
generation: Ada Lovelace
release_date: '2023-03-21'
signal_strength: medium
summary: NVIDIA datacenter GPU on the Ada Lovelace architecture with 24 GB of GDDR6 at 300 GB/s in a 72 W single-slot low-profile PCIe card.
aliases:
- NVIDIA L4
specifications:
  memory_gb: 24
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 300
  unit_kind: gpu
  compute_units: 7424
  compute_unit_type: CUDA Cores
  tensor_cores: 232
  rt_cores: 58
  tdp_watts: 72
  form_factor:
  - PCIe (low-profile)
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4N
performance:
  fp32_tflops: 30.3
  fp16_tflops: 121.0
  bf16_tflops: 121.0
  tf32_tflops: 60.0
  fp8_tflops: 242.0
  int8_tops: 242.0
  basis: dense
  performance_basis_note: dense; with sparsity NVIDIA lists twice these Tensor Core figures (TF32 120, FP16/BF16 242, FP8 485 TFLOPS, INT8 485 TOPS)
ml_capabilities:
  inference: true
  sparsity_support: true
  transformer_engine: true
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
  deepspeed: false
market:
  cloud_hourly_usd: 0.7946
  cloud_providers:
  - name: GCP
    instance_note: g2 instances
  - name: AWS
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Video
- AI
- Graphics
key_features:
- 24 GB GDDR6 with ECC, 300 GB/s
- 72 W, single-slot low-profile PCIe card
- Fourth-generation Tensor Cores with FP8
- Third-generation RT Cores
notable_users:
- Google Cloud (G2 VMs)
image: /images/gpus/nvidia-l4.jpg
tags:
- nvidia
- datacenter
- ada-lovelace
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/en-us/data-center/l4/
  title: NVIDIA L4 Tensor Core GPU (NVIDIA)
  trust: 0.95
- url: https://images.nvidia.com/aem-dam/Solutions/geforce/ada/nvidia-ada-gpu-architecture.pdf
  title: NVIDIA Ada GPU Architecture whitepaper (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-launches-inference-platforms-for-large-language-models-and-generative-ai-workloads
  title: NVIDIA Launches Inference Platforms for Large Language Models and Generative AI Workloads (NVIDIA Newsroom)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

NVIDIA datacenter GPU on the Ada Lovelace architecture with 24 GB of GDDR6 at 300 GB/s in a 72 W single-slot low-profile PCIe card.
