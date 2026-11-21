---
id: gpu/nvidia-v100-16gb
type: gpu
slug: nvidia-v100-16gb
schema_version: 1.4
title: V100 16GB
vendor: NVIDIA
segment: datacenter
series: Volta
generation: Volta
release_date: '2017-05-10'
signal_strength: low
summary: NVIDIA datacenter GPU on the Volta architecture with 16 GB of HBM2 at 900 GB/s in SXM2 and PCIe form factors.
aliases:
- NVIDIA V100 16GB
specifications:
  memory_gb: 16
  memory_type: HBM2
  memory_bandwidth_gb_per_s: 900
  unit_kind: gpu
  compute_units: 5120
  compute_unit_type: CUDA Cores
  tensor_cores: 640
  tdp_watts: 300
  form_factor:
  - SXM2
  - PCIe
  pcie_gen: 3.0
  interconnect:
    name: Second-generation NVLink
    bandwidth_gb_per_s: 300
  process_node:
    nodes_nm:
    - 12
    note: TSMC 12 nm FFN
performance:
  fp32_tflops: 15.7
  fp16_tflops: 125.0
  performance_basis_note: SXM2 figures; the FP16 figure is NVIDIA's "Tensor Performance". NVIDIA lists the PCIe card at 14 TFLOPS FP32 and 112 TFLOPS Tensor at 250 W
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: false
  transformer_engine: false
  multi_gpu_scaling:
    technology: NVLink
    max_units: 8
    note: up to eight V100 GPUs at up to 300 GB/s
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
  vllm: false
  deepspeed: true
market:
  cloud_hourly_usd: 0.7
  cloud_providers:
  - name: AWS
    instance_note: p3
  - name: GCP
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- AI
- High-performance computing (HPC)
- Graphics
key_features:
- 16 GB HBM2, 900 GB/s
- 640 Tensor Cores
- Second-generation NVLink, 300 GB/s (SXM2)
- ECC memory
notable_users:
- Oak Ridge National Laboratory (Summit)
image: /images/gpus/nvidia-v100-16gb.jpg
tags:
- nvidia
- datacenter
- volta
updated: '2026-11-21'
sources:
- url: https://images.nvidia.com/content/technologies/volta/pdf/tesla-volta-v100-datasheet-letter-fnl-web.pdf
  title: NVIDIA Tesla V100 GPU Accelerator data sheet (NVIDIA)
  trust: 0.95
- url: https://images.nvidia.com/content/volta-architecture/pdf/volta-architecture-whitepaper.pdf
  title: NVIDIA Tesla V100 GPU Architecture whitepaper (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-launches-revolutionary-volta-gpu-platform-fueling-next-era-of-ai-and-high-performance-computing
  title: NVIDIA Launches Revolutionary Volta GPU Platform (NVIDIA Newsroom)
  trust: 0.95
---

## Overview

NVIDIA datacenter GPU on the Volta architecture with 16 GB of HBM2 at 900 GB/s in SXM2 and PCIe form factors.
