---
id: glossary-term/hbm
type: glossary-term
slug: hbm
schema_version: 1.0
title: "HBM (High Bandwidth Memory)"
term: "HBM (High Bandwidth Memory)"
category: memory
examples: ["HBM2 on Tesla P100/V100", "HBM3 on H100", "HBM3e on H200 (141 GB)", "192 GB HBM3 on MI300X"]
related: [glossary-term/gddr6, glossary-term/memory-bandwidth, glossary-term/vram]
tags: [memory, hbm, bandwidth]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/High_Bandwidth_Memory", title: "High Bandwidth Memory — Wikipedia", trust: 0.8 }
---

## Definition
HBM is a stacked-DRAM memory technology in which multiple memory dies are stacked vertically and placed
next to the GPU on a silicon interposer, connected by a very wide (1024-bit-per-stack) bus. This yields
much higher bandwidth than the narrow, high-clock buses of GDDR. Generations are HBM2, HBM2e, HBM3, and
HBM3e.

## Why You Care
Large-model training and inference are usually memory-bound: performance is limited by how fast weights
and activations move to and from memory, not by raw compute. HBM's enormous bandwidth (multiple TB/s on
modern accelerators) is why datacenter AI GPUs use it despite the cost, while consumer cards use cheaper
GDDR. HBM capacity also sets how large a model fits on one device.
