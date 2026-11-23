---
id: guide/multi-gpu
type: guide
slug: multi-gpu
schema_version: 3.0
title: 'Multi-GPU: when one card is not enough'
page_section: background
order: 7
points:
- name: NVLink
  text: NVIDIA's GPU-to-GPU link, listed at 600 GB/s on the A100 and 900 GB/s on the H100 SXM and H200. NVIDIA lists NVLink as not supported on the GeForce RTX 4090 and RTX 5090.
- name: PCIe
  text: The standard host connection. NVIDIA lists PCIe Gen4 x16 at 64 GB/s bidirectional (L40S) and PCIe Gen5 at 128 GB/s (H100). PCI-SIG sets PCIe 5.0 at 32.0 GT/s and PCIe 6.0 at 64.0 GT/s, up to 256 GB/s on x16.
- name: Apple UltraFusion
  text: Apple's packaging that joins two M1 Max dies in the M1 Ultra with 2.5 TB/s of inter-processor bandwidth. Apple states software sees the M1 Ultra as one chip, with no code rewrite needed.
tags:
- gpu-buying-guide
- multi-gpu
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/en-us/data-center/a100/
  title: NVIDIA A100 Tensor Core GPU
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h200/
  title: NVIDIA H200 Tensor Core GPU
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/l40s/
  title: NVIDIA L40S GPU
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/
  title: NVIDIA GeForce RTX 4090
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5090/
  title: NVIDIA GeForce RTX 5090
  trust: 0.95
- url: https://pcisig.com/pci-express-6.0-specification
  title: PCI Express 6.0 Specification (PCI-SIG)
  trust: 0.95
- url: https://www.apple.com/newsroom/2022/03/apple-unveils-m1-ultra-the-worlds-most-powerful-chip-for-a-personal-computer/
  title: Apple unveils M1 Ultra (Apple Newsroom)
  trust: 0.95
---

## Overview

Several cards add memory; the link between them sets how fast they can share work.

## Takeaway

For multi-GPU training, plan on NVLink-capable datacenter GPUs, or rent them.
