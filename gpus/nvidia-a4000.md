---
id: gpu/nvidia-a4000
type: gpu
slug: nvidia-a4000
schema_version: 1.1
title: RTX A4000
vendor: NVIDIA
segment: workstation
series: Ampere
generation: Ampere
release_date: '2021-04-12'
signal_strength: low
summary: Budget-friendly professional GPU for entry-level ML development. Single-slot, low-power design.
aliases:
- NVIDIA RTX A4000
specifications:
  memory_gb: 16
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 448
  unit_kind: gpu
  compute_units: 6144
  compute_unit_type: CUDA Cores
  tensor_cores: 192
  rt_cores: 48
  tdp_watts: 140
  form_factor:
  - PCIe (single-slot)
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 8
performance:
  fp32_tflops: 19.2
  fp16_tflops: 38.4
  bf16_tflops: 38.4
  tf32_tflops: 38.4
  int8_tops: 153.4
ml_capabilities:
  inference: true
  training: false
  fine_tuning: true
  max_model_params_b_inference: 7
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
  deepspeed: false
market:
  msrp_usd: 1250
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Entry-level ML inference
- Light fine-tuning
- Compact workstations
key_features:
- Single-slot design
- 16 GB GDDR6
- Low power (140W)
- Affordable professional GPU
limitations:
- 16GB limits model size
- No NVLink
- Low memory bandwidth
notable_users:
- Small teams
- Individual developers
image: /images/gpus/nvidia-a4000.jpg
tags:
- nvidia
- workstation
- ampere
updated: '2026-11-19'
sources: []
---

## Overview

Budget-friendly professional GPU for entry-level ML development. Single-slot, low-power design.
