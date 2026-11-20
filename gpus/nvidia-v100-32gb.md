---
id: gpu/nvidia-v100-32gb
type: gpu
slug: nvidia-v100-32gb
schema_version: 1.1
title: V100 32GB
vendor: NVIDIA
segment: datacenter
series: Volta
generation: Volta
release_date: '2018-03-27'
signal_strength: low
summary: The GPU that launched the modern AI training era. Now legacy but still found in older cloud instances.
aliases:
- NVIDIA V100 32GB
specifications:
  memory_gb: 32
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
    name: NVLink 2.0
    bandwidth_gb_per_s: 300
  process_node:
    nodes_nm:
    - 12
performance:
  fp32_tflops: 15.7
  fp16_tflops: 125.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 13
  max_model_params_b_training: 5
  sparsity_support: false
  transformer_engine: false
  multi_gpu_scaling:
    technology: NVLink 2.0
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
  msrp_usd: 8000
  cloud_hourly_usd: 0.9
  cloud_providers:
  - name: AWS
    instance_note: p3
  - name: GCP
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Legacy ML workloads
- Smaller model training
- Budget cloud training
key_features:
- 32 GB HBM2
- First Tensor Core GPU
- NVLink 2.0
- Still available on clouds at lower cost
limitations:
- No BF16/TF32/FP8
- Older generation
- 32GB HBM2 is slow by modern standards
notable_users:
- Academic institutions
- Budget-conscious teams
image: /images/gpus/nvidia-v100-32gb.jpg
tags:
- nvidia
- datacenter
- volta
updated: '2026-11-20'
sources:
- url: https://images.nvidia.com/content/technologies/volta/pdf/tesla-volta-v100-datasheet-letter-fnl-web.pdf
  title: NVIDIA Tesla V100 GPU Accelerator data sheet (NVIDIA)
- url: https://nvidianews.nvidia.com/news/nvidia-launches-revolutionary-volta-gpu-platform-fueling-next-era-of-ai-and-high-performance-computing
  title: NVIDIA Launches Revolutionary Volta GPU Platform (NVIDIA Newsroom)
---

## Overview

The GPU that launched the modern AI training era. Now legacy but still found in older cloud instances.
