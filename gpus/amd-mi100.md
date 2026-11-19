---
id: gpu/amd-mi100
type: gpu
slug: amd-mi100
schema_version: 1.1
title: Instinct MI100
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA 1
release_date: '2020-11-16'
signal_strength: low
summary: AMD's first dedicated compute GPU architecture (CDNA). Largely superseded by MI250X and MI300X.
aliases:
- AMD Instinct MI100
specifications:
  memory_gb: 32
  memory_type: HBM2
  memory_bandwidth_gb_per_s: 1229
  unit_kind: gpu
  compute_units: 120
  compute_unit_type: Compute Units (CUs)
  tdp_watts: 300
  form_factor:
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: Infinity Fabric
  process_node:
    nodes_nm:
    - 7
performance:
  fp32_tflops: 23.1
  fp16_tflops: 184.6
  bf16_tflops: 92.3
  int8_tops: 184.6
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 13
  max_model_params_b_training: 5
  sparsity_support: false
  transformer_engine: false
  multi_gpu_scaling:
    technology: Infinity Fabric
framework_support:
  pytorch: true
  tensorflow: true
  jax: false
  onnx_runtime: true
  tensorrt: false
  directml: false
  mlx: false
  rocm: true
  oneapi: false
  triton: false
  vllm: false
  deepspeed: true
market:
  msrp_usd: 5000
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Legacy AMD AI workloads
- HPC + ML hybrid
key_features:
- 32 GB HBM2
- First CDNA architecture
- Matrix core FP16 and BF16
limitations:
- 32GB HBM2 is dated
- Limited software support
- First gen CDNA
notable_users:
- HPC clusters
image: /images/gpus/amd-mi100.png
tags:
- amd
- datacenter
- cdna-1
updated: '2026-11-19'
sources: []
---

## Overview

AMD's first dedicated compute GPU architecture (CDNA). Largely superseded by MI250X and MI300X.
