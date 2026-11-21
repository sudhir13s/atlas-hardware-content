---
id: gpu/amd-mi325x
type: gpu
slug: amd-mi325x
schema_version: 1.1
title: Instinct MI325X
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA 3
release_date: '2024-10-01'
signal_strength: high
summary: Memory-upgraded MI300X with 256GB HBM3e. Maximum single-GPU memory for AI inference workloads.
aliases:
- AMD Instinct MI325X
specifications:
  memory_gb: 256
  memory_type: HBM3e
  memory_bandwidth_gb_per_s: 6000
  unit_kind: gpu
  compute_units: 304
  compute_unit_type: Compute Units (CUs)
  tdp_watts: 750
  form_factor:
  - OAM
  pcie_gen: 5.0
  interconnect:
    name: Infinity Fabric
    bandwidth_gb_per_s: 896
  process_node:
    nodes_nm:
    - 5
    - 6
    note: 5nm + 6nm
performance:
  fp32_tflops: 163.4
  fp16_tflops: 1307.4
  bf16_tflops: 1307.4
  fp8_tflops: 2614.9
  int8_tops: 2614.9
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 230
  max_model_params_b_training: 90
  sparsity_support: true
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
  cloud_hourly_usd: 3.155
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Ultra-large model inference
- Memory-intensive training
- Single-GPU large model serving
key_features:
- 256 GB HBM3e
- 6 TB/s memory bandwidth
- Memory upgrade over MI300X
- Same CDNA 3 compute architecture
limitations:
- ROCm ecosystem less mature
- Same compute as MI300X
- High cost
notable_users:
- Microsoft Azure
- Cloud providers
image: /images/gpus/amd-mi325x.png
tags:
- amd
- datacenter
- cdna-3
updated: '2026-11-21'
sources:
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

Memory-upgraded MI300X with 256GB HBM3e. Maximum single-GPU memory for AI inference workloads.
