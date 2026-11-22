---
id: gpu/amd-rx-7900-xtx
type: gpu
slug: amd-rx-7900-xtx
schema_version: 2.0
title: Radeon RX 7900 XTX
vendor: AMD
segment: consumer
series: Radeon RX 7000
generation: RDNA 3
compute_platform: rocm
release_date: '2022-12-13'
signal_strength: low
summary: AMD consumer graphics card on the RDNA 3 architecture with 24 GB of GDDR6 at 960 GB/s and 96 compute units.
aliases:
- AMD Radeon RX 7900 XTX
specifications:
  memory_gb: 24
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 960
  unit_kind: gpu
  compute_units: 96
  compute_unit_type: Compute Units (CUs)
  tensor_cores: 192
  rt_cores: 96
  tdp_watts: 355
  form_factor:
  - PCIe
  process_node:
    nodes_nm:
    - 5
    - 6
    note: 5nm Graphics Compute Die, 6nm Memory Cache Dies
performance:
  fp32_tflops: 61.4
  fp16_tflops: 123
  performance_basis_note: FP32 is vector; FP16 is matrix (AMD lists FP16 vector at 61.4 TFLOPs)
ml_capabilities:
  inference: true
  training: false
  fine_tuning: false
  transformer_engine: false
market:
  msrp_usd: 999
  msrp_source: https://www.amd.com/en/newsroom/press-releases/2022-11-3-amd-unveils-world-s-most-advanced-gaming-graphics-.html
  msrp_announced: '2022-11-03'
  cloud_hourly_usd: 0.168
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
key_features:
- 24 GB GDDR6, 384-bit
- 96 compute units, 192 AI accelerators, 96 ray accelerators
- 96 MB AMD Infinity Cache
- 355 W typical board power
image: /images/gpus/amd-rx-7900-xtx.jpg
tags:
- amd
- consumer
- rdna-3
updated: '2026-11-22'
sources:
- url: https://www.amd.com/en/products/graphics/desktops/radeon/7000-series/amd-radeon-rx-7900xtx.html
  title: Radeon RX 7900 XTX (AMD)
  trust: 0.95
- url: https://www.amd.com/en/newsroom/press-releases/2022-11-3-amd-unveils-world-s-most-advanced-gaming-graphics-.html
  title: AMD Unveils World's Most Advanced Gaming Graphics Cards, Built on Groundbreaking AMD RDNA 3 Architecture with Chiplet Design (AMD)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

AMD consumer graphics card on the RDNA 3 architecture with 24 GB of GDDR6 at 960 GB/s and 96 compute units.
