---
id: gpu/amd-mi100
type: gpu
slug: amd-mi100
schema_version: 2.0
title: Instinct MI100
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA
compute_platform: rocm
release_date: '2020-11-16'
signal_strength: low
summary: AMD datacenter GPU on the CDNA architecture with 32 GB of HBM2 at 1.2 TB/s on a PCIe add-in card.
aliases:
- AMD Instinct MI100
specifications:
  memory_gb: 32
  memory_type: HBM2
  memory_bandwidth_gb_per_s: 1229
  unit_kind: gpu
  compute_units: 120
  compute_unit_type: Compute Units (CUs)
  tdp_watts: 300
  form_factor:
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: Infinity Fabric
    bandwidth_gb_per_s: 92
    note: per link; 3 links
  process_node:
    nodes_nm:
    - 7
    note: TSMC 7nm FinFET
performance:
  fp32_tflops: 23.1
  fp16_tflops: 184.6
  bf16_tflops: 92.3
  int8_tops: 92.3
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: false
  transformer_engine: false
  multi_gpu_scaling:
    technology: Infinity Fabric
market:
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- HPC
key_features:
- 32 GB HBM2
- 120 compute units
- Full-height, dual-slot PCIe card, passively cooled
- PCIe 4.0 x16
image: /images/gpus/amd-mi100.png
tags:
- amd
- datacenter
- cdna-1
updated: '2026-11-22'
sources:
- url: https://www.amd.com/en/products/accelerators/instinct/mi100.html
  title: AMD Instinct MI100 Accelerators (AMD)
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-business-docs/product-briefs/instinct-mi210-brochure.pdf
  title: AMD Instinct MI210 Accelerator brochure, MI100 memory bandwidth footnote (AMD)
  trust: 0.95
---

## Overview

AMD datacenter GPU on the CDNA architecture with 32 GB of HBM2 at 1.2 TB/s on a PCIe add-in card.
