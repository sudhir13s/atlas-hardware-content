---
id: gpu/apple-m1-ultra
type: gpu
slug: apple-m1-ultra
schema_version: 3.0
title: M1 Ultra
vendor: Apple
segment: workstation
series: Apple Silicon
generation: M1
compute_platform: apple-silicon
release_date: '2022-03-08'
signal_strength: low
summary: Apple system on a chip that joins two M1 Max dies with UltraFusion, with up to 128GB of unified memory at 800GB/s and up to a 64-core GPU, used in Mac Studio (2022).
aliases:
- Apple M1 Ultra
specifications:
  memory_gb: 128
  memory_kind: unified
  memory_options_gb:
  - 64
  - 128
  memory_bandwidth_gb_per_s: 800
  unit_kind: gpu
  compute_units: 64
  compute_unit_type: GPU Cores
  compute_unit_note: 48-core or 64-core GPU
  form_factor:
  - SoC (Mac Studio)
  interconnect:
    name: UltraFusion
    bandwidth_gb_per_s: 2500
    note: 2.5TB/s of low latency, inter-processor bandwidth
performance: {}
ml_capabilities:
  inference: true
  transformer_engine: false
market:
  observed_at: '2026-06-15'
  source: snapshot
key_features:
- Up to 128GB unified memory, 800GB/s
- 48-core or 64-core GPU
- 32-core Neural Engine, up to 22 trillion operations per second
- UltraFusion, 2.5TB/s inter-processor bandwidth
image: /images/gpus/apple-m1-ultra.jpg
tags:
- apple
- workstation
- m1
updated: '2026-11-23'
sources:
- url: https://www.apple.com/newsroom/2022/03/apple-unveils-m1-ultra-the-worlds-most-powerful-chip-for-a-personal-computer/
  title: Apple unveils M1 Ultra (Apple Newsroom)
  trust: 0.95
- url: https://support.apple.com/en-us/111900
  title: Mac Studio (2022) - Tech Specs (Apple Support)
  trust: 0.95
---


