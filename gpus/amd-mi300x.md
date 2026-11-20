---
id: gpu/amd-mi300x
type: gpu
slug: amd-mi300x
schema_version: 1.1
title: Instinct MI300X
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA 3
release_date: '2023-12-06'
signal_strength: high
summary: AMD's flagship AI GPU with industry-leading 192GB HBM3. The strongest NVIDIA alternative for datacenter AI.
aliases:
- AMD Instinct MI300X
specifications:
  memory_gb: 192
  memory_type: HBM3
  memory_bandwidth_gb_per_s: 5300
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
  max_model_params_b_inference: 175
  max_model_params_b_training: 70
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
  msrp_usd: 15000
  cloud_hourly_usd: 2.7156
  cloud_providers:
  - name: Microsoft Azure
    instance_note: ND MI300X
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Large model inference (memory advantage)
- Training with ROCm
- Alternative to NVIDIA datacenter
key_features:
- 192 GB HBM3 (largest GPU memory)
- 5.3 TB/s memory bandwidth
- Chiplet design (XCD + IOD)
- ROCm software ecosystem
limitations:
- ROCm ecosystem less mature than CUDA
- Fewer framework optimizations
- Higher TDP
notable_users:
- Microsoft Azure
- Meta
- Oracle Cloud
image: /images/gpus/amd-mi300x.png
tags:
- amd
- datacenter
- cdna-3
updated: '2026-11-20'
sources:
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

AMD's flagship AI GPU with industry-leading 192GB HBM3. The strongest NVIDIA alternative for datacenter AI.
