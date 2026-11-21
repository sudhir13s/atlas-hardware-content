---
id: gpu/nvidia-blackwell-ultra
type: gpu
slug: nvidia-blackwell-ultra
schema_version: 1.4
title: Blackwell Ultra B300
vendor: NVIDIA
segment: datacenter
series: Blackwell Ultra
generation: Blackwell Ultra
release_date: '2025-03-18'
signal_strength: high
summary: NVIDIA datacenter GPU on the Blackwell Ultra architecture with 288 GB of HBM3e at 8 TB/s in the SXM form factor.
aliases:
- NVIDIA Blackwell Ultra B300
specifications:
  memory_gb: 288
  memory_type: HBM3e
  memory_bandwidth_gb_per_s: 8000
  unit_kind: gpu
  tensor_cores: 640
  tdp_watts: 1400
  form_factor:
  - SXM
  pcie_gen: 6.0
  interconnect:
    name: Fifth-generation NVLink
    bandwidth_gb_per_s: 1800
    note: bidirectional per GPU
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4NP
performance:
  fp8_tflops: 5000.0
  basis: dense
  performance_basis_note: dense; with sparsity NVIDIA lists twice this (10 PFLOPS FP8).
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: Fifth-generation NVLink and NVLink 5 Switch (HGX B300)
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
  observed_at: '2026-06-15'
  source: snapshot
key_features:
- Two reticle-sized dies joined by a 10 TB/s NV-HBI link
- 288 GB HBM3e, 8 TB/s
- NVFP4 15 PFLOPS dense, 20 PFLOPS sparse
- Fifth-generation NVLink, 1.8 TB/s
- PCIe Gen 6 x16 host interface
- Up to 1,400 W TGP
image: /images/gpus/nvidia-blackwell-ultra.jpg
tags:
- nvidia
- datacenter
- blackwell-ultra
updated: '2026-11-21'
sources:
- url: https://developer.nvidia.com/blog/inside-nvidia-blackwell-ultra-the-chip-powering-the-ai-factory-era/
  title: 'Inside NVIDIA Blackwell Ultra: The Chip Powering the AI Factory Era (NVIDIA Technical Blog)'
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/hgx/
  title: NVIDIA HGX Platform, HGX B300 (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-blackwell-ultra-ai-factory-platform-paves-way-for-age-of-ai-reasoning
  title: NVIDIA Blackwell Ultra AI Factory Platform Paves Way for Age of AI Reasoning (NVIDIA Newsroom)
  trust: 0.95
---

## Overview

NVIDIA datacenter GPU on the Blackwell Ultra architecture with 288 GB of HBM3e at 8 TB/s in the SXM form factor.
