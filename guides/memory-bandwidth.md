---
id: guide/memory-bandwidth
type: guide
slug: memory-bandwidth
schema_version: 1.1
title: 'Memory Bandwidth: Why Speed Matters'
order: 2
memory_technologies:
- technology: HBM3e
  devices: H200, B200
  description: 4800-8000 GB/s — best for large-scale inference and training
- technology: HBM3
  devices: H100, A100, MI300X
  description: 2000-5300 GB/s — excellent for datacenter workloads
- technology: GDDR6X/GDDR7
  devices: RTX 4090, RTX 5090
  description: 1000-1800 GB/s — good for local inference
- technology: Unified LPDDR5X
  devices: Apple M-series
  description: 400-800 GB/s — lower bandwidth but no CPU↔GPU transfer penalty
tags:
- gpu-buying-guide
- memory-bandwidth
updated: '2026-11-19'
sources: []
---

## Overview

LLM inference is memory-bandwidth-bound, not compute-bound. The GPU spends most of its time reading model weights from memory, not doing math. Higher bandwidth = faster token generation.

## Takeaway

Rule: for inference, tokens/sec ≈ bandwidth / (2 × model_params_in_billions). An H100 (3350 GB/s) runs a 7B FP16 model at ~240 tok/s.
