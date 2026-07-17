---
id: name-decoder/amd
type: name-decoder
slug: amd
schema_version: 1.0
title: "AMD product-name decoder"
vendor: AMD
prefixes:
  - { symbol: "RX", meaning: "Radeon consumer gaming GPU" }
  - { symbol: "Instinct MI", meaning: "Datacenter compute accelerator (Machine Intelligence)" }
numbering: "Radeon RX: first digit = generation (5000 = RDNA 1, 6000 = RDNA 2, 7000 = RDNA 3); the next digits give the tier (900 > 800 > 700 > 600). Instinct: MI + number where the hundreds digit tracks the CDNA generation (MI100 = CDNA, MI200 = CDNA 2, MI300 = CDNA 3)."
suffixes:
  - { symbol: "XTX", meaning: "The highest bin in a Radeon generation" }
  - { symbol: "XT", meaning: "A high-performance bin, below XTX" }
  - { symbol: "GRE", meaning: "'Golden Rabbit Edition', a mid-tier bin" }
  - { symbol: "X / A (Instinct)", meaning: "MI300X = GPU-only accelerator; MI300A = APU (CPU + GPU on one package)" }
examples:
  - name: "Radeon RX 7900 XTX"
    parts:
      - { token: "RX", explains: "Radeon consumer gaming line" }
      - { token: "7900", explains: "7000-series generation (RDNA 3), top-tier 900 class" }
      - { token: "XTX", explains: "Highest bin of that model" }
  - name: "Instinct MI300X"
    parts:
      - { token: "Instinct MI", explains: "Datacenter compute accelerator" }
      - { token: "300", explains: "CDNA 3 generation" }
      - { token: "X", explains: "GPU-only variant (vs MI300A APU)" }
tags: [amd, naming, radeon, instinct]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Radeon_RX_7000_series", title: "Radeon RX 7000 series — Wikipedia", trust: 0.8 }
---

## How To Read
The prefix splits the two worlds: **RX** is a consumer Radeon gaming card, **Instinct MI** is a
datacenter accelerator. For **RX**, the leading digit is the generation (5/6/7 → RDNA 1/2/3) and the rest
is the tier (900 is top). The suffix is the performance bin: **XTX > XT > (base) > GRE**. For
**Instinct**, the hundreds digit tracks the CDNA generation (100/200/300), and the trailing letter
distinguishes a **GPU-only 'X'** part from an **APU 'A'** part that fuses CPU and GPU with unified memory.
