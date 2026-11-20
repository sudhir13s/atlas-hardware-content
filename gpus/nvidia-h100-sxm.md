---
id: gpu/nvidia-h100-sxm
type: gpu
slug: nvidia-h100-sxm
schema_version: 1.1
title: H100 SXM
vendor: NVIDIA
segment: datacenter
series: Hopper
generation: Hopper
release_date: '2022-09-20'
signal_strength: high
summary: NVIDIA's flagship AI datacenter GPU. The gold standard for LLM training and inference at scale.
aliases:
- NVIDIA H100 SXM
specifications:
  memory_gb: 80
  memory_type: HBM3
  memory_bandwidth_gb_per_s: 3350
  unit_kind: gpu
  compute_units: 16896
  compute_unit_type: CUDA Cores
  tensor_cores: 528
  tdp_watts: 700
  form_factor:
  - SXM5
  interconnect:
    name: NVLink 4.0
    bandwidth_gb_per_s: 900
  process_node:
    nodes_nm:
    - 4
performance:
  fp32_tflops: 67.0
  fp16_tflops: 989.0
  bf16_tflops: 989.0
  tf32_tflops: 495.0
  fp8_tflops: 1979.0
  int8_tops: 1979.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 70
  max_model_params_b_training: 30
  sparsity_support: true
  transformer_engine: true
  multi_gpu_scaling:
    technology: NVLink + NVSwitch
framework_support:
  pytorch: true
  tensorflow: true
  jax: true
  onnx_runtime: true
  tensorrt: true
  directml: false
  mlx: false
  rocm: false
  oneapi: false
  triton: true
  vllm: true
  deepspeed: true
market:
  msrp_usd: 30000
  cloud_hourly_usd: 3.5
  cloud_providers:
  - name: AWS
    instance_note: p5 instances
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Large-scale training
- LLM inference at scale
- Multi-GPU training
key_features:
- Transformer Engine with FP8
- 4th-gen NVLink (900 GB/s bidirectional)
- HBM3 memory
- Confidential Computing support
limitations:
- High power consumption (700W)
- Requires liquid cooling (SXM)
- Very expensive
notable_users:
- OpenAI
- Google
- Meta
- Microsoft Azure
image: /images/gpus/nvidia-h100-sxm.jpg
tags:
- nvidia
- datacenter
- hopper
updated: '2026-11-20'
sources:
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU (NVIDIA)
- url: https://nvidianews.nvidia.com/news/nvidia-announces-hopper-architecture-the-next-generation-of-accelerated-computing
  title: NVIDIA Announces Hopper Architecture (NVIDIA Newsroom)
---

## Overview

NVIDIA's flagship AI datacenter GPU. The gold standard for LLM training and inference at scale.
