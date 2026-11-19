---
id: guide/multi-gpu
type: guide
slug: multi-gpu
schema_version: 1.1
title: 'Multi-GPU: When One Card Isn''t Enough'
order: 5
interconnects:
- name: NVLink
  description: high-bandwidth GPU-to-GPU interconnect (600-900 GB/s). Required for efficient tensor parallelism. Available on datacenter GPUs (A100, H100, B200). Consumer GPUs do NOT have NVLink.
- name: PCIe
  description: standard GPU connection (32-64 GB/s). Works for pipeline parallelism but too slow for tensor parallelism. Using 2× RTX 4090 via PCIe gives 2× VRAM but not 2× speed.
- name: Apple UltraFusion
  description: die-to-die interconnect in M-series Ultra chips. Acts as one unified GPU. No software configuration needed.
tags:
- gpu-buying-guide
- multi-gpu
updated: '2026-11-19'
sources: []
---

## Takeaway

Rule: if you need multi-GPU for training, budget for NVLink-capable datacenter GPUs or use cloud. Consumer multi-GPU is a compromise.
