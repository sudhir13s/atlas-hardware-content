---
id: glossary-term/tdp
type: glossary-term
slug: tdp
schema_version: 3.0
title: TDP (Thermal Design Power)
term: TDP (Thermal Design Power)
category: power
examples:
- Max TDP up to 700 W (configurable) on H100 SXM
- Total graphics power 450 W on GeForce RTX 4090
- Typical board power 750 W peak on Instinct MI300X
related: []
tags:
- power
- tdp
- cooling
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/
  title: GeForce RTX 4090 specifications (NVIDIA)
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html
  title: AMD Instinct MI300X Accelerators (AMD)
  trust: 0.95
- url: https://www.amd.com/en/products/graphics/desktops/radeon/7000-series/amd-radeon-rx-7900xtx.html
  title: Radeon RX 7900 XTX specifications (AMD)
  trust: 0.95
---

## Definition

TDP (thermal design power) is a GPU's rated power in watts, as the maker publishes it. Makers name
the rating differently: NVIDIA lists maximum TDP for H100 and total graphics power for GeForce; AMD
lists typical board power.

## Why You Care

The rating drives the power supply, connectors and cooling you need. AMD, for example, recommends a
power supply of at least 800 W for a PC with the Radeon RX 7900 XTX (355 W typical board power).
