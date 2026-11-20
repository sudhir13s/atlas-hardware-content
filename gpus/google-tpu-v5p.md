---
id: gpu/google-tpu-v5p
type: gpu
slug: google-tpu-v5p
schema_version: 1.1
title: TPU v5p
vendor: Google
segment: datacenter
series: Cloud TPU
generation: v5p
release_date: '2023-12-06'
signal_strength: high
summary: Google's performance-optimized TPU for frontier model training. Scales to 8960 chips per pod.
aliases:
- Google TPU v5p
specifications:
  memory_gb: 95
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 2765
  unit_kind: gpu
  compute_units: 4
  compute_unit_type: Matrix Multiply Units (MXU)
  tensor_cores: 2
  tdp_watts: 250
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
  bf16_tflops: 459.0
  int8_tops: 918.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 40
  max_model_params_b_training: 15
  sparsity_support: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: ICI
    max_units: 8960
    note: up to 8960 chips per pod
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
  cloud_hourly_usd: 4.2
  cloud_providers:
  - name: Google Cloud
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Frontier model training
- Massive-scale distributed training
- Google-scale AI research
key_features:
- 95 GB HBM2e per chip
- 2x compute of TPU v4
- Up to 8960 chips per pod
- Largest-scale training platform
limitations:
- Google Cloud only
- Premium pricing
- JAX preferred
notable_users:
- Google DeepMind (Gemini)
- Google Research
image: /images/gpus/google-tpu-v5p.png
tags:
- google
- datacenter
- v5p
updated: '2026-11-20'
sources:
- url: https://docs.cloud.google.com/tpu/docs/v5p
  title: TPU v5p (Google Cloud documentation)
- url: https://epoch.ai/data/ml_hardware.csv
  title: Epoch AI, "Data on Machine Learning Hardware" (epoch.ai/data/machine-learning-hardware), CC BY; credit Epoch AI as the source.
---

## Overview

Google's performance-optimized TPU for frontier model training. Scales to 8960 chips per pod.
