---
id: gpu/nvidia-a100-80gb
type: gpu
slug: nvidia-a100-80gb
schema_version: 1.1
title: A100 80GB
vendor: NVIDIA
segment: datacenter
series: Ampere
generation: Ampere
release_date: '2021-06-28'
signal_strength: medium
summary: The workhorse of the AI revolution. Most widely deployed datacenter GPU for ML training and inference.
aliases:
- NVIDIA A100 80GB
specifications:
  memory_gb: 80
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 2039
  unit_kind: gpu
  compute_units: 6912
  compute_unit_type: CUDA Cores
  tensor_cores: 432
  tdp_watts: 400
  form_factor:
  - SXM4
  pcie_gen: 4.0
  interconnect:
    name: NVLink 3.0
    bandwidth_gb_per_s: 600
  process_node:
    nodes_nm:
    - 7
performance:
  fp32_tflops: 19.5
  fp16_tflops: 312.0
  bf16_tflops: 312.0
  tf32_tflops: 156.0
  int8_tops: 624.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 40
  max_model_params_b_training: 15
  sparsity_support: true
  transformer_engine: false
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
  cloud_hourly_usd: 1.6
  cloud_providers:
  - name: AWS
    instance_note: p4d instances
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Training medium models
- Multi-tenant inference (MIG)
- Fine-tuning LLMs
key_features:
- 80 GB HBM2e
- Multi-Instance GPU (MIG) for 7 GPU partitions
- 3rd-gen NVLink
- Structural sparsity (2:4)
limitations:
- No FP8 support
- Lower bandwidth than H100
- Previous generation
notable_users:
- Almost every AI lab (legacy fleet)
- AWS
- GCP
- Azure
image: /images/gpus/nvidia-a100-80gb.jpg
tags:
- nvidia
- datacenter
- ampere
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/a100/pdf/nvidia-a100-datasheet-us-nvidia-1758950-r4-web.pdf
  title: NVIDIA A100 Tensor Core GPU data sheet (NVIDIA)
- url: https://www.nvidia.com/en-us/data-center/a100/
  title: NVIDIA A100 Tensor Core GPU (NVIDIA)
---

## Overview

The workhorse of the AI revolution. Most widely deployed datacenter GPU for ML training and inference.
