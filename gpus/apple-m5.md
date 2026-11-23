---
id: gpu/apple-m5
type: gpu
slug: apple-m5
schema_version: 3.0
title: M5
vendor: Apple
segment: consumer
series: Apple Silicon
generation: M5
compute_platform: apple-silicon
release_date: '2025-10-15'
signal_strength: medium
summary: Apple system on a chip built on third-generation 3-nanometer technology, with 16GB, 24GB or 32GB of unified memory at 153GB/s in Macs and an 8-core or 10-core GPU, used in 14-inch MacBook Pro (M5) and MacBook Air (M5).
aliases:
- Apple M5
specifications:
  memory_gb: 32
  memory_kind: unified
  memory_options_gb:
  - 16
  - 24
  - 32
  memory_bandwidth_gb_per_s: 153
  unit_kind: gpu
  compute_units: 10
  compute_unit_type: GPU Cores
  compute_unit_note: 8-core or 10-core GPU
  form_factor:
  - SoC (MacBook Air / MacBook Pro)
  process_node:
    nodes_nm:
    - 3
    note: third-generation 3-nanometer technology
performance: {}
ml_capabilities:
  inference: true
market:
  observed_at: '2026-11-23'
  source: Apple publishes no chip price
key_features:
- 16GB, 24GB or 32GB unified memory, 153GB/s
- 8-core or 10-core GPU with a Neural Accelerator in each core
- 16-core Neural Engine
tags:
- apple
- consumer
- m5
updated: '2026-11-23'
sources:
- url: https://www.apple.com/newsroom/2025/10/apple-unleashes-m5-the-next-big-leap-in-ai-performance-for-apple-silicon/
  title: Apple unleashes M5, the next big leap in AI performance for Apple silicon (Apple Newsroom)
  trust: 0.95
- url: https://support.apple.com/en-us/125405
  title: MacBook Pro (14-inch, M5) - Tech Specs (Apple Support)
  trust: 0.95
- url: https://support.apple.com/en-us/126320
  title: MacBook Air (13-inch, M5) - Tech Specs (Apple Support)
  trust: 0.95
---


