---
id: gpu/nvidia-h100-pcie
type: gpu
slug: nvidia-h100-pcie
schema_version: 1.1
title: H100 PCIe
vendor: NVIDIA
segment: datacenter
series: Hopper
generation: Hopper
release_date: '2023-03-21'
signal_strength: high
summary: Air-cooled PCIe version of H100 with lower power draw, suitable for standard server racks.
aliases:
- NVIDIA H100 PCIe
specifications:
  memory_gb: 80
  memory_type: HBM3
  memory_bandwidth_gb_per_s: 2039
  unit_kind: gpu
  compute_units: 14592
  compute_unit_type: CUDA Cores
  tensor_cores: 456
  tdp_watts: 350
  form_factor:
  - PCIe
  pcie_gen: 5.0
  interconnect:
    name: NVLink 4.0
    bandwidth_gb_per_s: 600
  process_node:
    nodes_nm:
    - 4
performance:
  fp32_tflops: 51.2
  fp16_tflops: 756.0
  bf16_tflops: 756.0
  tf32_tflops: 378.0
  fp8_tflops: 1513.0
  int8_tops: 1513.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 70
  max_model_params_b_training: 25
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: NVLink
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
  cloud_hourly_usd: 2.5
  cloud_providers:
  - name: Various CSPs
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Inference workloads
- Training in air-cooled environments
- Enterprise AI
key_features:
- Transformer Engine with FP8
- PCIe form factor for standard servers
- HBM3 memory
- Lower TDP than SXM variant
limitations:
- Lower bandwidth than SXM variant
- Reduced NVLink bandwidth
notable_users:
- Enterprise customers
- Cloud providers
image: /images/gpus/nvidia-h100-pcie.jpg
tags:
- nvidia
- datacenter
- hopper
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU (NVIDIA)
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/gtcs22/data-center/h100/PB-11133-001_v01.pdf
  title: NVIDIA H100 PCIe GPU Product Brief (NVIDIA)
---

## Overview

Air-cooled PCIe version of H100 with lower power draw, suitable for standard server racks.
