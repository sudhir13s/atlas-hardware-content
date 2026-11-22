---
id: gpu/intel-arc-a770
type: gpu
slug: intel-arc-a770
schema_version: 2.0
title: Arc A770
vendor: Intel
segment: consumer
series: Arc
generation: Alchemist
compute_platform: intel-gpu
release_date: '2022-10-12'
signal_strength: low
summary: Intel Arc A-series desktop graphics card on the Xe-HPG microarchitecture with 16 GB of GDDR6 at 560 GB/s and 32 Xe-cores.
aliases:
- Intel Arc A770
specifications:
  memory_gb: 16
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 560
  unit_kind: gpu
  compute_units: 32
  compute_unit_type: Xe-cores
  rt_cores: 32
  tdp_watts: 225
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 6
    note: TSMC N6
performance:
  int8_tops: 262.0
  performance_basis_note: Intel lists GPU peak TOPS (INT8); Intel publishes no TFLOPS figures for this card.
ml_capabilities:
  inference: true
  training: false
  fine_tuning: false
  transformer_engine: false
market:
  msrp_usd: 349
  msrp_source: https://game.intel.com/us/stories/intel-arc-graphics-a7series-perf-per-dollar
  observed_at: '2026-06-15'
  source: snapshot
key_features:
- 16 GB GDDR6, 560 GB/s
- 32 Xe-cores with 512 Intel XMX engines
- 32 ray tracing units
- 225 W total board power
- Intel Extension for PyTorch (IPEX), oneAPI and OpenVINO support
image: /images/gpus/intel-arc-a770.jpg
tags:
- intel
- consumer
- alchemist
updated: '2026-11-22'
sources:
- url: https://www.intel.com/content/www/us/en/products/sku/229151/intel-arc-a770-graphics-16gb/specifications.html
  title: Intel Arc A770 Graphics (16GB) specifications (Intel)
  trust: 0.95
- url: https://game.intel.com/us/stories/intel-arc-graphics-a7series-perf-per-dollar
  title: 'Bringing Balance Back: Intel Arc A750 & A770 Performance per Dollar Details, available Oct 12th (Intel)'
  trust: 0.95
---

## Overview

Intel Arc A-series desktop graphics card on the Xe-HPG microarchitecture with 16 GB of GDDR6 at 560 GB/s and 32 Xe-cores.
