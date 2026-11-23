---
id: name-decoder/amd
type: name-decoder
slug: amd
schema_version: 3.0
title: AMD product-name decoder
vendor: AMD
prefixes:
- symbol: RX
  meaning: AMD Radeon RX desktop gaming graphics cards
- symbol: Instinct MI
  meaning: AMD Instinct data center accelerators
numbering: 'Radeon RX: the leading digit names the series, and each series uses one architecture (RX 5000 Series = RDNA, RX 6000 Series = RDNA 2, RX 7000 Series = RDNA 3). Within the RX 7000 Series a higher number has more compute units in AMD''s specification table (RX 7900 XTX 96, RX 7800 XT 60). Instinct: MI and a number; AMD groups the products into series, and its ROCm table gives each series one architecture (MI100 = CDNA, MI200 Series = CDNA 2, MI300 Series = CDNA 3).'
suffixes:
- symbol: XTX
  meaning: 'The higher-configured card of a pair: the RX 7900 XTX has 96 compute units, the RX 7900 XT 84'
- symbol: XT
  meaning: A card above the plain model (RX 6800 XT, 72 compute units, against 60 on the RX 6800), and below the XTX where one exists
- symbol: GRE
  meaning: Used on the RX 7900 GRE, which has 80 compute units, fewer than the RX 7900 XT
- symbol: X / A (Instinct)
  meaning: In the MI300 Series, the MI300X is a GPU accelerator and the MI300A an APU (accelerated processing unit) with CPU and GPU cores sharing one pool of HBM3 memory
examples:
- name: Radeon RX 7900 XTX
  parts:
  - token: RX
    explains: Radeon RX desktop gaming line
  - token: '7900'
    explains: RX 7000 Series (RDNA 3); the highest number in that series
  - token: XTX
    explains: The higher-configured card of the RX 7900 pair (96 compute units)
- name: Instinct MI300X
  parts:
  - token: Instinct MI
    explains: Data center accelerator line
  - token: '300'
    explains: MI300 Series, CDNA 3 architecture
  - token: X
    explains: The GPU accelerator of the series, as opposed to the MI300A APU
tags:
- amd
- naming
- radeon
- instinct
updated: '2026-11-21'
sources:
- url: https://rocm.docs.amd.com/en/latest/reference/gpu-specs.html
  title: AMD ROCm — GPU specifications
  trust: 0.95
- url: https://www.amd.com/en/support/downloads/drivers.html/graphics/radeon-rx/radeon-rx-5000-series/amd-radeon-rx-5700-xt.html
  title: AMD — Radeon RX 5700 XT specifications
  trust: 0.95
- url: https://www.amd.com/en/products/graphics/desktops/radeon/6000-series.html
  title: AMD Radeon RX 6000 Series graphics cards
  trust: 0.95
- url: https://rocm.docs.amd.com/en/docs-7.2.3/reference/gpu-arch-specs.html
  title: AMD ROCm 7.2.3 — GPU hardware specifications (includes RX 6000 Series)
  trust: 0.95
- url: https://www.amd.com/en/products/graphics/desktops/radeon/7000-series/amd-radeon-rx-7900-gre.html
  title: AMD — Radeon RX 7900 GRE specifications
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-tech-docs/data-sheets/amd-instinct-mi300a-data-sheet.pdf
  title: AMD Instinct MI300A APU data sheet
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-tech-docs/data-sheets/amd-instinct-mi300x-data-sheet.pdf
  title: AMD Instinct MI300X accelerator data sheet
  trust: 0.95
---

## How To Read

The prefix splits the two lines: **RX** is a Radeon desktop gaming card, **Instinct MI** a data center
accelerator.

- **RX:** the leading digit is the series (5/6/7 for RDNA, RDNA 2, RDNA 3) and the rest places the card
  within it. **XTX** and **XT** mark higher-configured cards than the plain model.
- **Instinct:** the number names the series, which maps to one CDNA generation. In the MI300 Series the
  **X** part is the GPU accelerator and the **A** part the APU that shares HBM3 memory between CPU and GPU.
