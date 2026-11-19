---
id: gpu/nvidia-rtx-5090
type: gpu
slug: nvidia-rtx-5090
schema_version: 1.1
title: GeForce RTX 5090
vendor: NVIDIA
segment: consumer
series: GeForce RTX 50
generation: Blackwell
release_date: '2025-01-30'
signal_strength: medium
summary: NVIDIA's flagship consumer GPU with 32GB GDDR7. Best consumer GPU for local AI workloads.
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
    - 5
performance:
  fp32_tflops: 104.8
  fp16_tflops: 209.6
  bf16_tflops: 209.6
  tf32_tflops: 209.6
  fp8_tflops: 838.0
  int8_tops: 838.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 20
  max_model_params_b_training: 7
  sparsity_support: true
  transformer_engine: false
framework_support:
  pytorch: true
  tensorflow: true
  jax: true
  onnx_runtime: true
  tensorrt: true
  directml: true
  mlx: false
  rocm: false
  oneapi: false
  triton: true
  vllm: true
  deepspeed: true
market:
  msrp_usd: 1999
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Local LLM inference
- Fine-tuning 7B models
- ML prototyping
- Gaming + AI
key_features:
- 32 GB GDDR7
- Blackwell consumer architecture
- FP8 support
- DLSS 4 with Multi Frame Generation
limitations:
- Consumer drivers
- No NVLink
- High power draw for desktop
- No ECC
notable_users:
- ML hobbyists
- Independent researchers
- AI enthusiasts
image: /images/gpus/nvidia-rtx-5090.jpg
tags:
- nvidia
- consumer
- blackwell
updated: '2026-11-19'
sources: []
---

## Overview

NVIDIA's flagship consumer GPU with 32GB GDDR7. Best consumer GPU for local AI workloads.
