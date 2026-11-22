---
id: gpu/intel-dc-gpu-max-1550
type: gpu
slug: intel-dc-gpu-max-1550
schema_version: 2.0
title: Data Center GPU Max 1550
vendor: Intel
segment: datacenter
series: Ponte Vecchio
generation: Xe-HPC
compute_platform: intel-gpu
release_date: '2023-01-10'
signal_strength: low
summary: Intel Data Center GPU Max Series GPU on the Xe-HPC microarchitecture with 128 GB of HBM2e at 3,276.8 GB/s and 128 Xe-cores in a 600 W OAM module.
aliases:
- Intel Data Center GPU Max 1550
specifications:
  memory_gb: 128
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 3276.8
  unit_kind: gpu
  compute_units: 128
  compute_unit_type: Xe-cores
  tensor_cores: 1024
  tdp_watts: 600
  form_factor:
  - OAM
  pcie_gen: 5.0
  interconnect:
    name: Intel Xe Link
    note: 16 Xe-Links per 2-stack GPU; 53 Gbps maximum link frequency
  process_node:
    nodes_nm:
    - 5
    note: Compute tiles on TSMC N5; base tile on Intel 7
performance: {}
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: Intel Xe Link
market:
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Artificial intelligence
- High performance computing
key_features:
- 128 GB HBM2e, 3,276.8 GB/s
- 128 Xe-cores with 1024 Intel XMX engines
- Intel Xe Link for multi-GPU scale-up
- PCIe Gen 5 x16 host interface
limitations:
- Intel lists expected discontinuance as January 2026
notable_users:
- Argonne National Laboratory (Aurora supercomputer)
image: /images/gpus/intel-dc-gpu-max-1550.jpg
tags:
- intel
- datacenter
- xe-hpc
updated: '2026-11-22'
sources:
- url: https://www.intel.com/content/www/us/en/products/sku/232873/intel-data-center-gpu-max-1550/specifications.html
  title: Intel Data Center GPU Max 1550 specifications (Intel)
  trust: 0.95
- url: https://download.intel.com/newsroom/archive/2025/en-us-2023-01-10-intel-launches-4th-gen-xeon-scalable-processors-max-series-cpus.pdf
  title: Intel Launches 4th Gen Xeon Scalable Processors, Max Series CPUs and GPUs (Intel)
  trust: 0.95
- url: https://download.intel.com/newsroom/2021/client-computing/intel-architecture-day-2021-fact-sheet.pdf
  title: Intel's Architecture Day 2021 Fact Sheet (Intel)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/docs/oneapi/optimization-guide-gpu/2024-0/intel-xe-gpu-architecture.html
  title: Intel Xe GPU Architecture, oneAPI GPU Optimization Guide (Intel)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/developer/articles/technical/accelerate-stable-diffusion-on-intel-gpus-openxla.html
  title: Accelerate Stable Diffusion on Intel GPUs with Intel Extension for OpenXLA (Intel)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/newsroom/news/aurora-supercomputer-blade-installation-complete.html
  title: Aurora Supercomputer Blade Installation Complete (Intel)
  trust: 0.95
---

## Overview

Intel Data Center GPU Max Series GPU on the Xe-HPC microarchitecture with 128 GB of HBM2e at 3,276.8 GB/s and 128 Xe-cores in a 600 W OAM module.
