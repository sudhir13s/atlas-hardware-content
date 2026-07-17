---
id: name-decoder/nvidia
type: name-decoder
slug: nvidia
schema_version: 1.0
title: "NVIDIA product-name decoder"
vendor: NVIDIA
prefixes:
  - { symbol: "RTX", meaning: "Consumer GeForce with RT Cores + Tensor Cores (ray tracing + DLSS)" }
  - { symbol: "GTX", meaning: "Legacy consumer GeForce without RT Cores" }
  - { symbol: "A / H / B / L", meaning: "Datacenter/pro cards named by architecture initial: A=Ampere, H=Hopper, B=Blackwell, L=Ada (L40)" }
numbering: "GeForce: first one or two digits = generation series (40 = Ada 40-series, 50 = Blackwell 50-series); last two digits = tier within the generation (90 > 80 > 70 > 60 > 50). Datacenter: the number is a product class (100 = flagship compute), not a generation."
suffixes:
  - { symbol: "Ti", meaning: "A higher-performance bin above the base model in the same tier" }
  - { symbol: "SUPER", meaning: "A mid-cycle refresh, faster than the original same-numbered card" }
  - { symbol: "SXM / PCIe", meaning: "Datacenter form factor: SXM = NVLink socket module; PCIe = add-in card" }
examples:
  - name: "GeForce RTX 4090"
    parts:
      - { token: "RTX", explains: "Consumer GeForce line with RT + Tensor Cores" }
      - { token: "40", explains: "40-series generation = Ada Lovelace architecture" }
      - { token: "90", explains: "Top consumer tier of that generation" }
  - name: "GeForce RTX 4080 SUPER"
    parts:
      - { token: "RTX", explains: "Consumer GeForce with RT + Tensor Cores" }
      - { token: "40", explains: "Ada Lovelace generation" }
      - { token: "80", explains: "High tier (below the 90 flagship)" }
      - { token: "SUPER", explains: "Mid-cycle refresh, faster than the original RTX 4080" }
  - name: "H100 SXM"
    parts:
      - { token: "H", explains: "Hopper architecture" }
      - { token: "100", explains: "Flagship datacenter compute class" }
      - { token: "SXM", explains: "NVLink socket module form factor (vs PCIe add-in card)" }
tags: [nvidia, naming, geforce, datacenter]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/GeForce_40_series", title: "GeForce 40 series — Wikipedia", trust: 0.8 }
---

## How To Read
Start with the prefix to learn the line: **RTX/GTX** is consumer GeForce, while a single **architecture
letter (A/H/B/L)** marks a datacenter or pro card. For GeForce, read the number as
**generation + tier**: the leading digit(s) give the series (40 = Ada, 50 = Blackwell) and the trailing
two digits give the tier (90 is the flagship, then 80/70/60). A **Ti** or **SUPER** suffix bumps the
card above its plain sibling. Datacenter numbers (100) denote a product class rather than a generation —
you infer the generation from the architecture letter, and the **SXM vs PCIe** suffix tells you the form
factor and whether it has NVLink.
