---
id: gpu/amd-mi250x
type: gpu
slug: amd-mi250x
schema_version: 1.1
title: Instinct MI250X
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA 2
release_date: '2021-11-08'
signal_strength: medium
summary: Dual-GCD GPU powering the Frontier exascale supercomputer. Strong HPC + AI convergence play.
aliases:
- AMD Instinct MI250X
specifications:
  memory_gb: 128
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 3277
  unit_kind: gpu
  compute_units: 220
  compute_unit_type: Compute Units (CUs)
  tdp_watts: 560
  form_factor:
  - OAM
  pcie_gen: 4.0
  interconnect:
    name: Infinity Fabric
    bandwidth_gb_per_s: 400
  process_node:
    nodes_nm:
    - 6
performance:
  fp32_tflops: 47.9
  fp16_tflops: 383.0
  bf16_tflops: 383.0
  int8_tops: 383.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 65
  max_model_params_b_training: 25
  sparsity_support: false
  transformer_engine: false
  multi_gpu_scaling:
    technology: Infinity Fabric
framework_support:
  pytorch: true
  tensorflow: true
  jax: true
  onnx_runtime: true
  tensorrt: false
  directml: false
  mlx: false
  rocm: true
  oneapi: false
  triton: true
  vllm: true
  deepspeed: true
market:
  msrp_usd: 12000
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- HPC + AI convergence
- Scientific computing
- Large-scale training with ROCm
key_features:
- 128 GB HBM2e (dual-GCD)
- Powers Frontier supercomputer
- High memory bandwidth
limitations:
- No FP8
- ROCm maturity
- Older CDNA generation
notable_users:
- Oak Ridge National Lab (Frontier)
- DOE
- National labs
image: /images/gpus/amd-mi250x.png
tags:
- amd
- datacenter
- cdna-2
updated: '2026-11-19'
sources: []
---

## Overview

Dual-GCD GPU powering the Frontier exascale supercomputer. Strong HPC + AI convergence play.
