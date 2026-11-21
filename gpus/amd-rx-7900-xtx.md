---
id: gpu/amd-rx-7900-xtx
type: gpu
slug: amd-rx-7900-xtx
schema_version: 1.3
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
  tensor_cores: 96
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
  msrp_source: https://www.amd.com/en/newsroom/press-releases/2022-11-3-amd-unveils-world-s-most-advanced-gaming-graphics-.html
  msrp_announced: '2022-11-03'
  cloud_hourly_usd: 0.168
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
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
updated: '2026-11-21'
sources:
- url: https://epoch.ai/data/ml_hardware.csv
  title: Epoch AI, "Data on Machine Learning Hardware" (epoch.ai/data/machine-learning-hardware), CC BY; credit Epoch AI as the source.
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

AMD's consumer flagship. 24GB VRAM is competitive but ROCm support for consumer cards lags behind CUDA.
