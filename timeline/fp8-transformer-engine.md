---
id: timeline-event/fp8-transformer-engine
type: timeline-event
slug: fp8-transformer-engine
schema_version: 1.0
title: "FP8 and the Transformer Engine arrive with Hopper"
date: 2022-03
vendor: NVIDIA
event_type: milestone
architecture_id: gpu-architecture/hopper
tags: [nvidia, hopper, fp8, transformer-engine, milestone]
updated: 2026-07-17
sources:
  - { url: "https://resources.nvidia.com/en-us-tensor-core/gtc22-whitepaper-hopper", title: "NVIDIA H100 Architecture Whitepaper", trust: 0.95 }
---

## Description
Hopper introduced 8-bit floating point (FP8) alongside the Transformer Engine, which tracks per-layer
statistics to switch between FP8 and FP16 automatically — roughly doubling transformer throughput while
preserving accuracy, and making 8-bit training practical.
