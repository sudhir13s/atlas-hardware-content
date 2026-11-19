---
id: gpu/nvidia-a10g
type: gpu
slug: nvidia-a10g
schema_version: 1.1
title: A10G
vendor: NVIDIA
segment: datacenter
series: Ampere
generation: Ampere
release_date: '2021-04-12'
signal_strength: medium
summary: Cost-effective Ampere GPU popular on AWS for inference and light fine-tuning workloads.
aliases:
- NVIDIA A10G
specifications:
  memory_gb: 24
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 600
  unit_kind: gpu
  compute_units: 9216
  compute_unit_type: CUDA Cores
  tensor_cores: 288
  rt_cores: 72
  tdp_watts: 150
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 8
performance:
  fp32_tflops: 31.2
  fp16_tflops: 62.5
  bf16_tflops: 62.5
  tf32_tflops: 62.5
  int8_tops: 250.0
ml_capabilities:
  inference: true
  training: false
  fine_tuning: true
  max_model_params_b_inference: 13
  sparsity_support: true
  transformer_engine: false
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
  cloud_hourly_usd: 0.76
  cloud_providers:
  - name: AWS
    instance_note: g5 instances
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Inference for small-medium models
- Fine-tuning 7B models
- AI + rendering combined
key_features:
- 24 GB GDDR6
- Low power (150W)
- Graphics + AI combined workloads
- Widely available on AWS
limitations:
- 24GB GDDR6 limits model size
- No NVLink
- Not suited for large-scale training
notable_users:
- AWS g5 instances
- Startups
- SaaS inference
image: /images/gpus/nvidia-a10g.jpg
tags:
- nvidia
- datacenter
- ampere
updated: '2026-11-19'
sources: []
---

## Overview

Cost-effective Ampere GPU popular on AWS for inference and light fine-tuning workloads.
