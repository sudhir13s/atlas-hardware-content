---
id: gpu/amd-mi325x
type: gpu
slug: amd-mi325x
schema_version: 1.4
title: Instinct MI325X
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA 3
release_date: '2024-10-10'
signal_strength: high
summary: AMD datacenter GPU on the CDNA 3 architecture with 256 GB of HBM3E at 6 TB/s in the OAM form factor.
aliases:
- AMD Instinct MI325X
specifications:
  memory_gb: 256
  memory_type: HBM3E
  memory_bandwidth_gb_per_s: 6000
  unit_kind: gpu
  compute_units: 304
  compute_unit_type: Compute Units (CUs)
  tdp_watts: 1000
  form_factor:
  - OAM
  pcie_gen: 5.0
  interconnect:
    name: Infinity Fabric
    bandwidth_gb_per_s: 896
    note: 7x 128 GB/s links per GPU; 128 GB/s bidirectional between each GPU
  process_node:
    nodes_nm:
    - 5
    - 6
    note: TSMC 5nm | 6nm FinFET
performance:
  fp32_tflops: 163.4
  fp16_tflops: 1307.4
  bf16_tflops: 1307.4
  fp8_tflops: 2614.9
  int8_tops: 2614.9
  basis: dense
  performance_basis_note: dense; with structured sparsity AMD lists twice these for FP16, BF16, FP8 and INT8
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
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
  cloud_hourly_usd: 3.155
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- AI training
- AI inference
key_features:
- 256 GB HBM3E
- 6 TB/s memory bandwidth
- 304 compute units
- PCIe 5.0 x16
image: /images/gpus/amd-mi325x.png
tags:
- amd
- datacenter
- cdna-3
updated: '2026-11-21'
sources:
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi325x.html
  title: AMD Instinct MI325X Accelerators (AMD)
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-tech-docs/product-briefs/instinct-mi325x-datasheet.pdf
  title: AMD Instinct MI325X Accelerator data sheet (AMD)
  trust: 0.95
- url: https://ir.amd.com/news-events/press-releases/detail/1218/amd-unveils-leadership-ai-solutions-at-advancing-ai-2024
  title: AMD Unveils Leadership AI Solutions at Advancing AI 2024 (AMD)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

AMD datacenter GPU on the CDNA 3 architecture with 256 GB of HBM3E at 6 TB/s in the OAM form factor.
