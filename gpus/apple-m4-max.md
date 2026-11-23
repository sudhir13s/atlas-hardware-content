---
id: gpu/apple-m4-max
type: gpu
slug: apple-m4-max
schema_version: 3.0
title: M4 Max
vendor: Apple
segment: workstation
series: Apple Silicon
generation: M4
compute_platform: apple-silicon
release_date: '2024-10-30'
signal_strength: medium
summary: Apple system on a chip built on second-generation 3-nanometer technology, with up to 128GB of unified memory at up to 546GB/s and a 32-core or 40-core GPU, used in MacBook Pro (2024) and Mac Studio (2025).
aliases:
- Apple M4 Max
specifications:
  memory_gb: 128
  memory_note: 128GB with the 16-core CPU; 546GB/s with the 40-core GPU, 410GB/s with the 32-core GPU
  memory_kind: unified
  memory_options_gb:
  - 36
  - 48
  - 64
  - 128
  memory_bandwidth_gb_per_s: 546
  unit_kind: gpu
  compute_units: 40
  compute_unit_type: GPU Cores
  compute_unit_note: 32-core or 40-core GPU
  form_factor:
  - SoC (MacBook Pro / Mac Studio)
  process_node:
    nodes_nm:
    - 3
    note: second-generation 3-nanometer technology
performance: {}
ml_capabilities:
  inference: true
  transformer_engine: false
market:
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Working with large language models
key_features:
- Up to 128GB unified memory, up to 546GB/s
- 32-core or 40-core GPU with hardware-accelerated ray tracing
- 16-core Neural Engine
- Thunderbolt 5, up to 120Gb/s
image: /images/gpus/apple-m4-max.jpg
tags:
- apple
- workstation
- m4
updated: '2026-11-23'
sources:
- url: https://www.apple.com/newsroom/2024/10/apple-introduces-m4-pro-and-m4-max/
  title: Apple introduces M4 Pro and M4 Max (Apple Newsroom)
  trust: 0.95
- url: https://support.apple.com/en-us/121553
  title: MacBook Pro (14-inch, M4 Pro or M4 Max, 2024) - Tech Specs (Apple Support)
  trust: 0.95
- url: https://support.apple.com/en-us/122211
  title: Mac Studio (2025) - Tech Specs (Apple Support)
  trust: 0.95
---


