---
id: glossary-term/gddr6
type: glossary-term
slug: gddr6
schema_version: 1.0
title: "GDDR6 / GDDR6X / GDDR7"
term: "GDDR6 / GDDR6X / GDDR7"
category: memory
examples: ["GDDR6 on Radeon RX 7900 XTX and Arc A770", "GDDR6X on GeForce RTX 3090 and RTX 4090", "GDDR7 on GeForce RTX 5090"]
related: [glossary-term/hbm, glossary-term/vram]
tags: [memory, gddr, consumer]
updated: '2026-11-21'
sources:
  - { url: "https://www.jedec.org/news/pressreleases/jedec-publishes-gddr7-graphics-memory-standard", title: "JEDEC Publishes GDDR7 Graphics Memory Standard (JEDEC)", trust: 0.95 }
  - { url: "https://www.micron.com/products/memory/graphics-memory/gddr6x", title: "GDDR6X (Micron)", trust: 0.95 }
  - { url: "https://www.intel.com/content/www/us/en/products/sku/229151/intel-arc-a770-graphics-16gb/specifications.html", title: "Intel Arc A770 Graphics (16GB) specifications (Intel)", trust: 0.95 }
  - { url: "https://www.amd.com/en/products/graphics/desktops/radeon/7000-series/amd-radeon-rx-7900xtx.html", title: "Radeon RX 7900 XTX specifications (AMD)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/geforce/graphics-cards/30-series/rtx-3090-3090ti/", title: "GeForce RTX 3090 specifications (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/", title: "GeForce RTX 4090 specifications (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5090/", title: "GeForce RTX 5090 specifications (NVIDIA)", trust: 0.95 }
---

## Definition
GDDR (Graphics Double Data Rate) is the memory on consumer graphics cards, on a bus such as 256-bit
(Arc A770) or 384-bit (GeForce RTX 4090). Micron's GDDR6X uses PAM4 signaling, and JEDEC's GDDR7 uses
PAM3; both are multi-level signaling that raises the data rate per pin.

## Why You Care
On a consumer card, GDDR capacity and bandwidth are the memory figures to compare: 24 GB and up to
960 GB/s on the Radeon RX 7900 XTX, 16 GB and 560 GB/s on the Arc A770. Datacenter accelerators use
HBM instead, with bandwidth in TB/s.
