---
id: gpu/amd-mi210
type: gpu
slug: amd-mi210
schema_version: 2.0
title: Instinct MI210
vendor: AMD
segment: datacenter
series: Instinct
generation: CDNA 2
compute_platform: rocm
release_date: '2022-03-22'
signal_strength: low
summary: AMD datacenter GPU on the CDNA 2 architecture with 64 GB of HBM2e at 1.6 TB/s on a PCIe add-in card.
aliases:
- AMD Instinct MI210
specifications:
  memory_gb: 64
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 1638
  unit_kind: gpu
  compute_units: 104
  compute_unit_type: Compute Units (CUs)
  tdp_watts: 300
  form_factor:
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: Infinity Fabric
    bandwidth_gb_per_s: 300
    note: 3 links of 100 GB/s; peak GPU-to-GPU bandwidth per card
  process_node:
    nodes_nm:
    - 6
    note: 6nm FinFET
performance:
  fp32_tflops: 22.6
  fp16_tflops: 181.0
  bf16_tflops: 181.0
  int8_tops: 181.0
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
market:
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- HPC
- AI
key_features:
- 64 GB HBM2e
- One graphics compute die (GCD)
- Full-height, full-length dual-slot PCIe card, passively cooled
- 300 W TDP
limitations:
- No TF32, FP8 or sparsity support
image: /images/gpus/amd-mi210.png
tags:
- amd
- datacenter
- cdna-2
updated: '2026-11-22'
sources:
- url: https://www.amd.com/en/products/accelerators/instinct/mi200/mi210.html
  title: AMD Instinct MI210 Accelerators (AMD)
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-business-docs/product-briefs/instinct-mi210-brochure.pdf
  title: AMD Instinct MI210 Accelerator brochure (AMD)
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-business-docs/white-papers/amd-cdna2-white-paper.pdf
  title: AMD CDNA 2 Architecture white paper (AMD)
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-tech-docs/data-sheets/amd-instinct-mi300x-data-sheet.pdf
  title: AMD Instinct MI300X Accelerator data sheet, MI200 series data-type note (AMD)
  trust: 0.95
---

## Overview

AMD datacenter GPU on the CDNA 2 architecture with 64 GB of HBM2e at 1.6 TB/s on a PCIe add-in card.
