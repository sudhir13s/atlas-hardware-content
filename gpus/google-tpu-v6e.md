---
id: gpu/google-tpu-v6e
type: gpu
slug: google-tpu-v6e
schema_version: 1.1
title: TPU v6e (Trillium)
vendor: Google
segment: datacenter
series: Cloud TPU
generation: v6e (Trillium)
release_date: '2024-08-01'
signal_strength: high
summary: Google's latest cost-efficient TPU generation (Trillium). Nearly 5x compute improvement over v5e at similar cost.
aliases:
- Google TPU v6e (Trillium)
specifications:
  memory_gb: 32
  memory_type: HBM
  memory_bandwidth_gb_per_s: 1640
  unit_kind: gpu
  compute_units: 2
  compute_unit_type: Matrix Multiply Units (MXU)
  tdp_watts: 150
  form_factor:
  - Custom (Google pod)
  interconnect:
    name: ICI
    note: Inter-Chip Interconnect
  process_node:
    nodes_nm:
    - 5
performance:
  bf16_tflops: 918.0
  int8_tops: 1836.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 15
  max_model_params_b_training: 7
  sparsity_support: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: ICI
    max_units: 256
    note: up to 256 chips per pod
framework_support:
  pytorch: true
  tensorflow: true
  jax: true
  onnx_runtime: false
  tensorrt: false
  directml: false
  mlx: false
  rocm: false
  oneapi: false
  triton: false
  vllm: false
  deepspeed: false
market:
  cloud_hourly_usd: 1.5
  cloud_providers:
  - name: Google Cloud
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Cost-effective inference at scale
- Medium-scale training
- Efficient serving
key_features:
- 4.7x improvement in peak compute per chip over v5e
- Cost-optimized for inference
- Improved energy efficiency
- 5nm process node
limitations:
- Google Cloud only
- 32GB per chip
- Inference-optimized, not for frontier training
notable_users:
- Google Cloud AI customers
image: /images/gpus/google-tpu-v6e.png
tags:
- google
- datacenter
- v6e-trillium
updated: '2026-11-20'
sources:
- url: https://docs.cloud.google.com/tpu/docs/v6e
  title: TPU v6e (Google Cloud documentation)
---

## Overview

Google's latest cost-efficient TPU generation (Trillium). Nearly 5x compute improvement over v5e at similar cost.
