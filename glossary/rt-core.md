---
id: glossary-term/rt-core
type: glossary-term
slug: rt-core
schema_version: 1.0
title: "RT Core"
term: "RT Core"
category: compute
examples: ["RT Cores introduced with Turing", "3rd-generation RT Cores on Ada Lovelace", "AMD Ray Accelerators; Intel Ray Tracing Units"]
related: [glossary-term/cuda-core, glossary-term/tensor-core]
tags: [compute, rt-core, ray-tracing]
updated: '2026-11-21'
sources:
  - { url: "https://developer.nvidia.com/blog/nvidia-turing-architecture-in-depth/", title: "NVIDIA Turing Architecture In-Depth (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/geforce/ada-lovelace-architecture/", title: "NVIDIA Ada Lovelace Architecture (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/", title: "GeForce RTX 4090 specifications (NVIDIA)", trust: 0.95 }
  - { url: "https://www.amd.com/en/products/graphics/desktops/radeon/7000-series/amd-radeon-rx-7900xtx.html", title: "Radeon RX 7900 XTX specifications (AMD)", trust: 0.95 }
  - { url: "https://www.intel.com/content/www/us/en/developer/articles/technical/introduction-to-the-xe-hpg-architecture.html", title: "Introduction to the Xe-HPG Architecture (Intel)", trust: 0.95 }
---

## Definition
An RT Core is NVIDIA's dedicated ray-tracing unit; NVIDIA states it accelerates bounding volume
hierarchy (BVH) traversal and ray/triangle intersection testing. AMD lists Ray Accelerators on its
Radeon cards, and Intel has one Ray Tracing Unit per Xe-core.

## Why You Care
RT Cores accelerate ray tracing, a graphics workload. They are listed separately from CUDA cores and
Tensor Cores on the same specification sheet (GeForce RTX 4090), so their count is not an AI figure.
