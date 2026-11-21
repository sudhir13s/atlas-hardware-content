---
id: gpu/amd-mi250x
type: gpu
slug: amd-mi250x
schema_version: 1.4
title: Instinct MI250X
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA 2
release_date: '2021-11-08'
signal_strength: medium
summary: AMD datacenter GPU on the CDNA 2 architecture with two graphics compute dies and 128 GB of HBM2e at 3.2 TB/s in the OAM form factor.
aliases:
- AMD Instinct MI250X
specifications:
  memory_gb: 128
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 3277
  unit_kind: gpu
  compute_units: 220
  compute_unit_type: Compute Units (CUs)
  tdp_watts: 560
  form_factor:
  - OAM
  pcie_gen: 4.0
  interconnect:
    name: Infinity Fabric
    bandwidth_gb_per_s: 100
    note: per link; 8 links
  process_node:
    nodes_nm:
    - 6
    note: TSMC 6nm FinFET
performance:
  fp32_tflops: 47.9
  fp16_tflops: 383.0
  bf16_tflops: 383.0
  int8_tops: 383.0
  basis: dense
  performance_basis_note: dense; AMD states the MI200 series does not support sparsity
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: false
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
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- HPC
- AI
key_features:
- 128 GB HBM2e
- Two graphics compute dies (GCDs)
- 220 compute units
- Eight Infinity Fabric links
limitations:
- No TF32, FP8 or sparsity support
notable_users:
- Oak Ridge National Laboratory (Frontier)
image: /images/gpus/amd-mi250x.png
tags:
- amd
- datacenter
- cdna-2
updated: '2026-11-21'
sources:
- url: https://www.amd.com/en/products/accelerators/instinct/mi200/mi250x.html
  title: AMD Instinct MI250X Accelerators (AMD)
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-business-docs/white-papers/amd-cdna2-white-paper.pdf
  title: AMD CDNA 2 Architecture white paper (AMD)
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-tech-docs/data-sheets/amd-instinct-mi300x-data-sheet.pdf
  title: AMD Instinct MI300X Accelerator data sheet, MI200 series data-type note (AMD)
  trust: 0.95
- url: https://ir.amd.com/news-events/press-releases/detail/1032/new-amd-instinct-mi200-series-accelerators-bring-leadership-hpc-and-ai-performance-to-power-exascale-systems-and-more
  title: New AMD Instinct MI200 Series Accelerators Bring Leadership HPC and AI Performance to Power Exascale Systems and More (AMD)
  trust: 0.95
---

## Overview

AMD datacenter GPU on the CDNA 2 architecture with two graphics compute dies and 128 GB of HBM2e at 3.2 TB/s in the OAM form factor.
