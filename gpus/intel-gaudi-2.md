---
id: gpu/intel-gaudi-2
type: gpu
slug: intel-gaudi-2
schema_version: 2.0
title: Gaudi 2
vendor: Intel
segment: datacenter
series: Gaudi
generation: Gaudi 2
compute_platform: intel-gaudi
release_date: '2022-05-10'
signal_strength: medium
summary: Intel AI accelerator with 96 GB of HBM2e at 2.46 TB/s, 24 Tensor Processor Cores and 24 integrated 100 GbE RoCE ports, in the OAM form factor.
aliases:
- Intel Gaudi 2
specifications:
  memory_gb: 96
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 2460
  unit_kind: gpu
  compute_units: 24
  compute_unit_type: Tensor Processor Cores (TPC)
  tdp_watts: 600
  form_factor:
  - OAM
  pcie_gen: 4.0
  interconnect:
    name: 24x 100GbE RoCE RDMA
    bandwidth_gb_per_s: 600
    note: bidirectional
  process_node:
    nodes_nm:
    - 7
performance:
  bf16_tflops: 432.0
  fp8_tflops: 865.0
  performance_basis_note: Intel lists these as matrix engine (MME) TFLOPS; Intel lists 11 BF16 vector TFLOPS.
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: Ethernet-based
    note: RoCE v2; 21 ports connect the 8 cards of a server all-to-all, 3 ports scale out
market:
  cloud_hourly_usd: 1.7
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Deep learning training
- Deep learning inference
key_features:
- 96 GB HBM2e
- 24 x 100GbE RoCE RDMA NICs on chip
- 24 Tensor Processor Cores and 2 matrix engines
- FP8 support
- SynapseAI software stack
image: /images/gpus/intel-gaudi-2.jpg
tags:
- intel
- datacenter
- gaudi-2
updated: '2026-11-22'
sources:
- url: https://cdrdv2-public.intel.com/817486/gaudi-3-ai-accelerator-white-paper.pdf
  title: Intel Gaudi 3 AI Accelerator White Paper, Gaudi 2 and Gaudi 3 comparison (Intel)
  trust: 0.95
- url: https://cdrdv2-public.intel.com/845118/gaudi-3-ai-accelerator-30-3-30.pdf
  title: Intel Gaudi 3 AI Accelerator overview, Gaudi 2 and Gaudi 3 product specs (Intel)
  trust: 0.95
- url: https://download.intel.com/newsroom/archive/2025/de-de-2022-05-10-intels-habana-labs-launches-secondgeneration-ai-processors-for-training-and-inferencing.pdf
  title: Intel's Habana Labs Launches Second-Generation AI Processors for Training and Inferencing (Intel)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/developer/articles/technical/habana-gaudi2-processor-for-deep-learning.html
  title: Habana Gaudi2 AI Processor for Deep Learning Gets Even Better (Intel)
  trust: 0.95
---

## Overview

Intel AI accelerator with 96 GB of HBM2e at 2.46 TB/s, 24 Tensor Processor Cores and 24 integrated 100 GbE RoCE ports, in the OAM form factor.
