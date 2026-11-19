---
id: gpu/nvidia-gb200
type: gpu
slug: nvidia-gb200
schema_version: 1.1
title: GB200 Grace Blackwell Superchip
vendor: NVIDIA
segment: datacenter
series: Blackwell
generation: Blackwell
release_date: '2025-03-01'
signal_strength: high
summary: NVIDIA's complete AI superchip combining Grace ARM CPU with two Blackwell GPUs for maximum AI throughput.
aliases:
- NVIDIA GB200 Grace Blackwell Superchip
specifications:
  memory_gb: 384
  memory_type: HBM3e + LPDDR5X
  memory_bandwidth_gb_per_s: 16000
  unit_kind: module
  gpus_per_module: 2
  compute_units: 36864
  compute_unit_type: CUDA Cores
  compute_unit_note: 2x B200 GPUs
  tensor_cores: 1152
  tdp_watts: 2700
  form_factor:
  - Superchip Module
  interconnect:
    name: NVLink 5.0 + Grace CPU coherent link
    bandwidth_gb_per_s: 1800
    note: 1800 GB/s per GPU
  process_node:
    nodes_nm:
    - 4
    note: 4nm (GPU) + 4nm (Grace CPU)
performance:
  fp32_tflops: 180.0
  fp16_tflops: 4500.0
  bf16_tflops: 4500.0
  tf32_tflops: 2250.0
  fp8_tflops: 9000.0
  int8_tops: 9000.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 400
  max_model_params_b_training: 175
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: NVLink 5.0 + NVSwitch + Grace interconnect
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
  msrp_usd: 70000
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Trillion-parameter model training
- Full-stack AI supercomputing
- Massive inference farms
key_features:
- Combined Grace CPU + 2x Blackwell GPUs
- 384 GB total memory across module
- 9 PetaFLOPS FP8 per superchip
- Unified memory architecture with CPU
limitations:
- 2.7kW power per module
- Requires liquid cooling rack infrastructure
- Extremely high cost
notable_users:
- OpenAI
- Microsoft
- Meta
- xAI
- Oracle Cloud
image: /images/gpus/nvidia-gb200.jpg
tags:
- nvidia
- datacenter
- blackwell
updated: '2026-11-19'
sources: []
---

## Overview

NVIDIA's complete AI superchip combining Grace ARM CPU with two Blackwell GPUs for maximum AI throughput.
