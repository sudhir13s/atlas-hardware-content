---
id: gpu/apple-m2-ultra
type: gpu
slug: apple-m2-ultra
schema_version: 3.0
title: M2 Ultra
vendor: Apple
segment: workstation
series: Apple Silicon
generation: M2
compute_platform: apple-silicon
release_date: '2023-06-05'
signal_strength: medium
summary: Apple system on a chip built on a second-generation 5-nanometer process, with up to 192GB of unified memory at 800GB/s and a 60-core or 76-core GPU, used in Mac Studio and Mac Pro (2023).
aliases:
- Apple M2 Ultra
specifications:
  memory_gb: 192
  memory_kind: unified
  memory_options_gb:
  - 64
  - 128
  - 192
  memory_bandwidth_gb_per_s: 800
  unit_kind: gpu
  compute_units: 76
  compute_unit_type: GPU Cores
  compute_unit_note: 60-core or 76-core GPU
  form_factor:
  - SoC (Mac Studio / Mac Pro)
  interconnect:
    name: UltraFusion
    bandwidth_gb_per_s: 2500
    note: over 2.5TB/s of low-latency interprocessor bandwidth
  process_node:
    nodes_nm:
    - 5
    note: second-generation 5-nanometer process
performance: {}
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  transformer_engine: false
market:
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Machine learning training in a single system
key_features:
- Up to 192GB unified memory, 800GB/s
- 60-core or 76-core GPU
- 32-core Neural Engine, 31.6 trillion operations per second
- UltraFusion, over 2.5TB/s interprocessor bandwidth
image: /images/gpus/apple-m2-ultra.jpg
tags:
- apple
- workstation
- m2
updated: '2026-11-23'
sources:
- url: https://www.apple.com/newsroom/2023/06/apple-introduces-m2-ultra/
  title: Apple introduces M2 Ultra (Apple Newsroom)
  trust: 0.95
- url: https://support.apple.com/en-us/111835
  title: Mac Studio (2023) - Tech Specs (Apple Support)
  trust: 0.95
---


