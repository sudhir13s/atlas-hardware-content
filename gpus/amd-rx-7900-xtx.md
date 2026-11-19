---
id: gpu/amd-rx-7900-xtx
type: gpu
slug: amd-rx-7900-xtx
schema_version: 1.1
title: Radeon RX 7900 XTX
vendor: AMD
segment: consumer
series: Radeon RX 7000
generation: RDNA 3
release_date: '2022-12-13'
signal_strength: low
summary: AMD's consumer flagship. 24GB VRAM is competitive but ROCm support for consumer cards lags behind CUDA.
aliases:
- AMD Radeon RX 7900 XTX
specifications:
  memory_gb: 24
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 960
  unit_kind: gpu
  compute_units: 96
  compute_unit_type: Compute Units (CUs)
  rt_cores: 96
  tdp_watts: 355
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 5
    - 6
    note: 5nm + 6nm
performance:
  fp32_tflops: 61.4
  fp16_tflops: 122.8
ml_capabilities:
  inference: true
  training: false
  fine_tuning: false
  max_model_params_b_inference: 13
  sparsity_support: false
  transformer_engine: false
framework_support:
  pytorch: true
  tensorflow: true
  jax: false
  onnx_runtime: true
  tensorrt: false
  directml: true
  mlx: false
  rocm: true
  oneapi: false
  triton: false
  vllm: false
  deepspeed: false
market:
  msrp_usd: 999
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Budget local inference
- ROCm experimentation
- Gaming + light AI
key_features:
- 24 GB GDDR6
- RDNA 3 chiplet design
- ROCm support (improving)
- Competitive pricing
limitations:
- ROCm on consumer cards is immature
- No BF16 on RDNA 3
- Limited ML framework support
notable_users:
- Budget-conscious hobbyists
image: /images/gpus/amd-rx-7900-xtx.jpg
tags:
- amd
- consumer
- rdna-3
updated: '2026-11-19'
sources: []
---

## Overview

AMD's consumer flagship. 24GB VRAM is competitive but ROCm support for consumer cards lags behind CUDA.
