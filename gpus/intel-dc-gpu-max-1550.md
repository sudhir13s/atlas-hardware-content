---
id: gpu/intel-dc-gpu-max-1550
type: gpu
slug: intel-dc-gpu-max-1550
schema_version: 1.1
title: Data Center GPU Max 1550
vendor: Intel
segment: datacenter
series: Ponte Vecchio
generation: Xe HPC
release_date: '2023-01-10'
signal_strength: low
summary: Intel's HPC GPU powering the Aurora supercomputer. Primarily HPC-focused with growing AI capabilities.
aliases:
- Intel Data Center GPU Max 1550
specifications:
  memory_gb: 128
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 3277
  unit_kind: gpu
  compute_units: 128
  compute_unit_type: Xe Cores
  tensor_cores: 1024
  tdp_watts: 600
  form_factor:
  - OAM
  pcie_gen: 5.0
  interconnect:
    name: Xe Link
    bandwidth_gb_per_s: 128
    note: 128 GB/s per link
  process_node:
    nodes_nm:
    - 5
    note: Multi-tile (TSMC 5nm + Intel 7)
performance:
  fp32_tflops: 52.0
  fp16_tflops: 839.0
  bf16_tflops: 839.0
  tf32_tflops: 419.0
  int8_tops: 1678.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 65
  max_model_params_b_training: 25
  sparsity_support: false
  transformer_engine: false
  multi_gpu_scaling:
    technology: Xe Link
framework_support:
  pytorch: true
  tensorflow: true
  jax: false
  onnx_runtime: true
  tensorrt: false
  directml: false
  mlx: false
  rocm: false
  oneapi: true
  triton: false
  vllm: false
  deepspeed: true
market:
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- HPC + AI convergence
- Scientific computing
- oneAPI ecosystem
key_features:
- 128 GB HBM2e
- Multi-tile design (Ponte Vecchio)
- Xe Link for multi-GPU
- Powers Aurora supercomputer
limitations:
- Very limited commercial availability
- Niche software ecosystem
- Primarily for national labs
notable_users:
- Argonne National Lab (Aurora supercomputer)
image: /images/gpus/intel-dc-gpu-max-1550.jpg
tags:
- intel
- datacenter
- xe-hpc
updated: '2026-11-20'
sources:
- url: https://epoch.ai/data/ml_hardware.csv
  title: Epoch AI, "Data on Machine Learning Hardware" (epoch.ai/data/machine-learning-hardware), CC BY; credit Epoch AI as the source.
---

## Overview

Intel's HPC GPU powering the Aurora supercomputer. Primarily HPC-focused with growing AI capabilities.
