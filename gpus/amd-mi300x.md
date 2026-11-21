---
id: gpu/amd-mi300x
type: gpu
slug: amd-mi300x
schema_version: 1.4
title: Instinct MI300X
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA 3
release_date: '2023-12-06'
signal_strength: high
summary: AMD datacenter GPU on the CDNA 3 architecture with 192 GB of HBM3 at 5.3 TB/s in the OAM form factor.
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
  cloud_hourly_usd: 2.7156
  cloud_providers:
  - name: Microsoft Azure
    instance_note: ND MI300X
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Generative AI
- HPC
key_features:
- 192 GB HBM3
- 5.3 TB/s memory bandwidth
- 304 compute units
- Eight XCDs per OAM module
- PCIe 5.0 x16
notable_users:
- Microsoft Azure
- Meta
- Oracle Cloud Infrastructure
image: /images/gpus/amd-mi300x.png
tags:
- amd
- datacenter
- cdna-3
updated: '2026-11-21'
sources:
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html
  title: AMD Instinct MI300X Accelerators (AMD)
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-tech-docs/data-sheets/amd-instinct-mi300x-data-sheet.pdf
  title: AMD Instinct MI300X Accelerator data sheet (AMD)
  trust: 0.95
- url: https://www.amd.com/en/newsroom/press-releases/2023-12-6-amd-showcases-growing-momentum-for-amd-powered-ai-.html
  title: AMD Showcases Growing Momentum for AMD Powered AI Solutions from the Data Center to PCs (AMD)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
---

## Overview

AMD datacenter GPU on the CDNA 3 architecture with 192 GB of HBM3 at 5.3 TB/s in the OAM form factor.
