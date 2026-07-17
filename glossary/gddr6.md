---
id: glossary-term/gddr6
type: glossary-term
slug: gddr6
schema_version: 1.0
title: "GDDR6 / GDDR6X / GDDR7"
term: "GDDR6 / GDDR6X / GDDR7"
category: memory
examples: ["GDDR6 on RX 7900 XTX and Arc A770", "GDDR6X on RTX 3090/4090", "GDDR7 on RTX 5090"]
related: [glossary-term/hbm, glossary-term/vram]
tags: [memory, gddr, consumer]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/GDDR6_SDRAM", title: "GDDR6 SDRAM — Wikipedia", trust: 0.8 }
---

## Definition
GDDR (Graphics Double Data Rate) is the standard memory on consumer GPUs: discrete DRAM chips soldered
around the GPU on the board, connected by a fast but relatively narrow bus (e.g. 256–384 bits). GDDR6X
(NVIDIA/Micron) and GDDR7 push per-pin data rates higher using multi-level signaling.

## Why You Care
GDDR is far cheaper and easier to manufacture than HBM, which is why gaming and prosumer cards use it —
but it delivers lower total bandwidth for the same power. When choosing hardware for AI, a consumer card's
GDDR bandwidth and capacity (e.g. 24 GB) are often the binding constraint on model size and inference
speed, versus the multi-TB/s HBM of datacenter parts.
