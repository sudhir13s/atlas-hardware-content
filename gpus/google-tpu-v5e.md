---
id: gpu/google-tpu-v5e
type: gpu
slug: google-tpu-v5e
schema_version: 1.1
title: TPU v5e
vendor: Google
segment: datacenter
series: Cloud TPU
generation: v5e
release_date: '2023-08-29'
signal_strength: medium
summary: Cost-optimized TPU for inference and medium-scale training. Half the cost per chip of TPU v4.
aliases:
- Google TPU v5e
specifications:
  memory_gb: 16
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 819
  unit_kind: gpu
  compute_units: 1
  compute_unit_type: Matrix Multiply Units (MXU)
  tensor_cores: 1
  tdp_watts: 100
  form_factor:
  - Custom (Google pod)
  interconnect:
    name: ICI
    note: Inter-Chip Interconnect
  process_node:
    nodes_nm:
    - 7
performance:
  bf16_tflops: 197.0
  int8_tops: 394.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 7
  max_model_params_b_training: 3
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
  cloud_hourly_usd: 1.2
  cloud_providers:
  - name: Google Cloud
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Cost-effective inference
- Medium-scale training
- Fine-tuning on Google Cloud
key_features:
- Cost-optimized TPU
- Half the price per chip of v4
- Up to 256 chips per pod
- Best for inference and medium training
limitations:
- 16GB per chip is limiting
- Google Cloud only
- Less compute than v5p
notable_users:
- Google Cloud customers
- Startups on GCP
image: /images/gpus/google-tpu-v5e.png
tags:
- google
- datacenter
- v5e
updated: '2026-11-20'
sources:
- url: https://epoch.ai/data/ml_hardware.csv
  title: Epoch AI, "Data on Machine Learning Hardware" (epoch.ai/data/machine-learning-hardware), CC BY; credit Epoch AI as the source.
---

## Overview

Cost-optimized TPU for inference and medium-scale training. Half the cost per chip of TPU v4.
