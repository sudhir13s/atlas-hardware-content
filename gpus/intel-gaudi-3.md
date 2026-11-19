---
id: gpu/intel-gaudi-3
type: gpu
slug: intel-gaudi-3
schema_version: 1.1
title: Gaudi 3
vendor: Intel
segment: datacenter
series: Gaudi
generation: Gaudi 3
release_date: '2024-04-09'
signal_strength: medium
summary: Intel's next-gen AI accelerator with 2x Gaudi 2 performance. Competing directly with H100 on price-performance.
aliases:
- Intel Gaudi 3
specifications:
  memory_gb: 128
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 3700
  unit_kind: gpu
  compute_units: 64
  compute_unit_type: Tensor Processor Cores (TPC)
  tdp_watts: 900
  form_factor:
  - OAM
  pcie_gen: 5.0
  interconnect:
    name: 24x 200GbE RoCE RDMA
  process_node:
    nodes_nm:
    - 5
performance:
  fp32_tflops: 90.0
  fp16_tflops: 900.0
  bf16_tflops: 900.0
  fp8_tflops: 1835.0
  int8_tops: 1835.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 70
  max_model_params_b_training: 30
  sparsity_support: false
  transformer_engine: false
  multi_gpu_scaling:
    technology: Ethernet-based
    note: 200GbE RDMA
framework_support:
  pytorch: true
  tensorflow: true
  jax: false
  onnx_runtime: false
  tensorrt: false
  directml: false
  mlx: false
  rocm: false
  oneapi: true
  triton: false
  vllm: true
  deepspeed: true
market:
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Cost-effective NVIDIA alternative
- Large-scale training
- Cloud inference
key_features:
- 128 GB HBM2e
- 2x performance over Gaudi 2
- 24x 200GbE integrated networking
- FP8 with enhanced precision
limitations:
- New platform with maturing ecosystem
- Fewer benchmarks available
- Intel ecosystem dependency
notable_users:
- Intel partners
- Cloud providers
image: /images/gpus/intel-gaudi-3.jpg
tags:
- intel
- datacenter
- gaudi-3
updated: '2026-11-19'
sources: []
---

## Overview

Intel's next-gen AI accelerator with 2x Gaudi 2 performance. Competing directly with H100 on price-performance.
