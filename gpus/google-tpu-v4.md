---
id: gpu/google-tpu-v4
type: gpu
slug: google-tpu-v4
schema_version: 1.1
title: TPU v4
vendor: Google
segment: datacenter
series: Cloud TPU
generation: v4
release_date: '2022-07-01'
signal_strength: high
summary: Google's custom AI accelerator optimized for JAX. Scales to 4096 chips in a pod for massive training runs.
aliases:
- Google TPU v4
specifications:
  memory_gb: 32
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 1200
  unit_kind: gpu
  compute_units: 2
  compute_unit_type: Matrix Multiply Units (MXU)
  tdp_watts: 175
  form_factor:
  - Custom (Google pod)
  interconnect:
    name: ICI
    bandwidth_gb_per_s: 600
    note: Inter-Chip Interconnect, 4800 Gbps per chip
  process_node:
    nodes_nm:
    - 7
performance:
  bf16_tflops: 275.0
  int8_tops: 275.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 13
  max_model_params_b_training: 5
  sparsity_support: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: ICI
    max_units: 4096
    note: up to 4096 chips in a pod
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
  cloud_hourly_usd: 3.22
  cloud_providers:
  - name: Google Cloud
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Google Cloud training at scale
- JAX-native workloads
- Research requiring massive parallelism
key_features:
- Optimized for JAX and TensorFlow
- ICI interconnect for massive scale
- Up to 4096 chips per pod
- SparseCore for sparse operations
limitations:
- Google Cloud only
- 32GB per chip is limiting
- Best with JAX, okay with PyTorch
notable_users:
- Google DeepMind
- Google Research
- Anthropic
image: /images/gpus/google-tpu-v4.png
tags:
- google
- datacenter
- v4
updated: '2026-11-20'
sources:
- url: https://docs.cloud.google.com/tpu/docs/v4
  title: TPU v4 (Google Cloud documentation)
---

## Overview

Google's custom AI accelerator optimized for JAX. Scales to 4096 chips in a pod for massive training runs.
