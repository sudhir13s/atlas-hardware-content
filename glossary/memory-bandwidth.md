---
id: glossary-term/memory-bandwidth
type: glossary-term
slug: memory-bandwidth
schema_version: 1.0
title: "Memory Bandwidth"
term: "Memory Bandwidth"
category: memory
examples: ["~3.35 TB/s on H100 SXM (HBM3)", "~1 TB/s on RTX 4090 (GDDR6X)", "~5.3 TB/s on MI300X"]
related: [glossary-term/hbm, glossary-term/vram]
tags: [memory, bandwidth, performance]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Memory_bandwidth", title: "Memory bandwidth — Wikipedia", trust: 0.8 }
---

## Definition
Memory bandwidth is the rate at which data moves between the GPU's compute units and its VRAM, measured
in gigabytes or terabytes per second. It is set by the memory technology, the bus width, and the clock
(bandwidth ≈ bus-width × data-rate).

## Why You Care
Much of AI inference — especially generating one token at a time — is memory-bandwidth-bound, not
compute-bound: the GPU must stream the entire model's weights from VRAM for each token. That is why two
cards with similar TFLOPS can differ greatly in tokens-per-second, and why HBM's high bandwidth matters
so much for serving large models.
