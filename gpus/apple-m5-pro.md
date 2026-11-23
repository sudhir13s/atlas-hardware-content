---
id: gpu/apple-m5-pro
type: gpu
slug: apple-m5-pro
schema_version: 3.0
title: M5 Pro
vendor: Apple
segment: workstation
series: Apple Silicon
generation: M5
compute_platform: apple-silicon
release_date: '2026-03-03'
signal_strength: medium
summary: Apple system on a chip built on third-generation 3-nanometer technology, with 24GB, 48GB or 64GB of unified memory at 307GB/s and a 16-core or 20-core GPU, used in MacBook Pro (M5 Pro) and Mac mini (M5 Pro).
aliases:
- Apple M5 Pro
specifications:
  memory_gb: 64
  memory_note: 64GB with the 20-core GPU in MacBook Pro
  memory_kind: unified
  memory_options_gb:
  - 24
  - 48
  - 64
  memory_bandwidth_gb_per_s: 307
  unit_kind: gpu
  compute_units: 20
  compute_unit_type: GPU Cores
  compute_unit_note: 16-core or 20-core GPU
  form_factor:
  - SoC (MacBook Pro / Mac mini)
  process_node:
    nodes_nm:
    - 3
    note: two third-generation 3-nanometer dies
performance: {}
ml_capabilities:
  inference: true
market:
  observed_at: '2026-11-23'
  source: Apple publishes no chip price
key_features:
- 24GB, 48GB or 64GB unified memory, 307GB/s
- 16-core or 20-core GPU with a Neural Accelerator in each core
- 16-core Neural Engine
- Thunderbolt 5
tags:
- apple
- workstation
- m5
updated: '2026-11-23'
sources:
- url: https://www.apple.com/newsroom/2026/03/apple-debuts-m5-pro-and-m5-max-to-supercharge-the-most-demanding-pro-workflows/
  title: Apple debuts M5 Pro and M5 Max to supercharge the most demanding pro workflows (Apple Newsroom)
  trust: 0.95
- url: https://support.apple.com/en-us/126318
  title: MacBook Pro (14-inch, M5 Pro or M5 Max) - Tech Specs (Apple Support)
  trust: 0.95
- url: https://support.apple.com/en-us/128108
  title: Mac mini (M6 or M5 Pro) - Tech Specs (Apple Support)
  trust: 0.95
---


