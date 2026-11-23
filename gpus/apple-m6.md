---
id: gpu/apple-m6
type: gpu
slug: apple-m6
schema_version: 3.0
title: M6
vendor: Apple
segment: consumer
series: Apple Silicon
generation: M6
compute_platform: apple-silicon
release_date: '2026-08-25'
signal_strength: medium
summary: Apple system on a chip built on a 2-nanometer process, with 16GB, 24GB or 32GB of unified memory at up to 170GB/s and a 12-core GPU, used in Mac mini (M6) and 14-inch MacBook Pro (M6).
aliases:
- Apple M6
specifications:
  memory_gb: 32
  memory_note: 170GB/s with 24GB or 32GB, 153GB/s with 16GB
  memory_kind: unified
  memory_options_gb:
  - 16
  - 24
  - 32
  memory_bandwidth_gb_per_s: 170
  unit_kind: gpu
  compute_units: 12
  compute_unit_type: GPU Cores
  form_factor:
  - SoC (Mac mini / MacBook Pro)
  process_node:
    nodes_nm:
    - 2
    note: Apple's first 2 nm chip
performance: {}
ml_capabilities:
  inference: true
market:
  observed_at: '2026-11-23'
  source: Apple publishes no chip price
key_features:
- 16GB, 24GB or 32GB unified memory, up to 170GB/s
- 12-core GPU with a Neural Accelerator in each core
- Dual 16-core Neural Engine
tags:
- apple
- consumer
- m6
updated: '2026-11-23'
sources:
- url: https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/
  title: Apple introduces M6 and M5 Ultra for a big leap in performance and AI compute (Apple Newsroom)
  trust: 0.95
- url: https://support.apple.com/en-us/128108
  title: Mac mini (M6 or M5 Pro) - Tech Specs (Apple Support)
  trust: 0.95
- url: https://support.apple.com/en-us/148300
  title: MacBook Pro (14-inch, M6) - Tech Specs (Apple Support)
  trust: 0.95
---


