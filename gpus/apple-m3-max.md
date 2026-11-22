---
id: gpu/apple-m3-max
type: gpu
slug: apple-m3-max
schema_version: 2.0
title: M3 Max
vendor: Apple
segment: workstation
series: Apple Silicon
generation: M3
compute_platform: apple-silicon
release_date: '2023-10-30'
signal_strength: medium
summary: Apple system on a chip built on a 3-nanometer process, with up to 128GB of unified memory at up to 400GB/s and a 30-core or 40-core GPU, used in MacBook Pro (Nov 2023).
aliases:
- Apple M3 Max
specifications:
  memory_gb: 128
  memory_note: 128GB with the 16-core CPU; 400GB/s with the 40-core GPU, 300GB/s with the 30-core GPU
  memory_kind: unified
  memory_bandwidth_gb_per_s: 400
  unit_kind: gpu
  compute_units: 40
  compute_unit_type: GPU Cores
  compute_unit_note: 30-core or 40-core GPU
  form_factor:
  - SoC (MacBook Pro)
  process_node:
    nodes_nm:
    - 3
    note: 3-nanometer process technology
performance: {}
ml_capabilities:
  inference: true
  transformer_engine: false
market:
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Working with large transformer models
key_features:
- Up to 128GB unified memory, up to 400GB/s
- 30-core or 40-core GPU with hardware-accelerated ray tracing
- 16-core Neural Engine
- 92 billion transistors
image: /images/gpus/apple-m3-max.jpg
tags:
- apple
- workstation
- m3
updated: '2026-11-22'
sources:
- url: https://www.apple.com/newsroom/2023/10/apple-unveils-m3-m3-pro-and-m3-max-the-most-advanced-chips-for-a-personal-computer/
  title: Apple unveils M3, M3 Pro, and M3 Max (Apple Newsroom)
  trust: 0.95
- url: https://support.apple.com/en-us/117737
  title: MacBook Pro (16-inch, Nov 2023) - Tech Specs (Apple Support)
  trust: 0.95
---

## Overview

Apple system on a chip built on a 3-nanometer process, with up to 128GB of unified memory at up to 400GB/s and a 30-core or 40-core GPU, used in MacBook Pro (Nov 2023).
