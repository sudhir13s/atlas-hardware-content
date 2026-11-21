---
id: gpu/amd-mi210
type: gpu
slug: amd-mi210
schema_version: 1.1
title: Instinct MI210
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA 2
release_date: '2022-03-22'
signal_strength: low
summary: PCIe-compatible single-GCD variant of MI250X for standard server deployments.
aliases:
- AMD Instinct MI210
specifications:
  memory_gb: 64
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 1638
  unit_kind: gpu
  compute_units: 104
  compute_unit_type: Compute Units (CUs)
  tdp_watts: 300
  form_factor:
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: Infinity Fabric
  process_node:
    nodes_nm:
    - 6
performance:
  fp32_tflops: 22.6
  fp16_tflops: 181.0
  bf16_tflops: 181.0
  int8_tops: 181.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 30
  max_model_params_b_training: 10
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
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- PCIe-compatible AMD AI
- HPC workloads
- ROCm development
key_features:
- 64 GB HBM2e
- PCIe form factor (air-cooled)
- Single-GCD variant of MI250
limitations:
- Single GCD (half MI250X)
- No FP8
- ROCm ecosystem
notable_users:
- HPC clusters
- Research institutions
image: /images/gpus/amd-mi210.png
tags:
- amd
- datacenter
- cdna-2
updated: '2026-11-21'
sources:
- url: https://www.amd.com/en/products/accelerators/instinct/mi200/mi210.html
  title: AMD Instinct MI210 Accelerators (AMD)
---

## Overview

PCIe-compatible single-GCD variant of MI250X for standard server deployments.
