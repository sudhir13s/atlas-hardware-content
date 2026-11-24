---
id: gpu/nvidia-h200
type: gpu
slug: nvidia-h200
schema_version: 3.0
title: H200
vendor: NVIDIA
segment: datacenter
generation: Hopper
architecture: gpu-architecture/hopper
compute_platform: cuda
compute_capability: 9.0
release_date: '2023-11-13'
signal_strength: high
summary: NVIDIA datacenter GPU on the Hopper architecture with 141 GB of HBM3e at 4.8 TB/s in the SXM form factor.
aliases:
- NVIDIA H200
specifications:
  memory_gb: 141
  memory_type: HBM3e
  memory_bandwidth_gb_per_s: 4800
  unit_kind: gpu
  tdp_watts: 700
  form_factor:
  - SXM
  pcie_gen: 5.0
  interconnect:
    name: Fourth-generation NVLink
    bandwidth_gb_per_s: 900
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4N
performance:
  fp32_tflops: 67.0
  fp16_tflops: 989.5
  bf16_tflops: 989.5
  tf32_tflops: 494.5
  fp8_tflops: 1979.0
  int8_tops: 1979.0
  basis: dense
  performance_basis_note: dense; NVIDIA lists the Tensor Core figures "With sparsity" at twice these (TF32 989, FP16/BF16 1,979, FP8 3,958 TFLOPS, INT8 3,958 TOPS); FP32 is a non-Tensor Core figure. NVIDIA marks the H200 specifications preliminary.
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: Fourth-generation NVLink and third-generation NVSwitch (HGX H200)
market:
  cloud_hourly_usd: 4.75
  cloud_providers:
  - name: AWS
  - name: GCP
  - name: Azure
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Generative AI and large language models
- High-performance computing
key_features:
- 141 GB HBM3e, 4.8 TB/s
- NVLink 900 GB/s, PCIe Gen5 128 GB/s
- Up to 700 W TDP (configurable)
- Up to 7 MIG instances at 18 GB each
- Confidential Computing
image: /images/gpus/nvidia-h200.jpg
tags:
- nvidia
- datacenter
- hopper
updated: '2026-11-24'
sources:
- url: https://www.nvidia.com/en-us/data-center/h200/
  title: NVIDIA H200 GPU (NVIDIA)
  trust: 0.95
- url: https://docs.nvidia.com/enterprise-reference-architectures/hgx-ai-factory-h100-h200-b200/latest/components.html
  title: NVIDIA HGX AI Factory (HGX H100, H200, B200) Components (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/technologies/hopper-architecture/
  title: NVIDIA Hopper Architecture (NVIDIA)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://nvidianews.nvidia.com/news/nvidia-supercharges-hopper-the-worlds-leading-ai-computing-platform
  title: NVIDIA Supercharges Hopper, the World's Leading AI Computing Platform (NVIDIA Newsroom, November 13, 2023)
  trust: 0.95
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---


