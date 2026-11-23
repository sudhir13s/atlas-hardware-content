---
id: glossary-term/cuda-core
type: glossary-term
slug: cuda-core
schema_version: 3.0
title: CUDA Core
term: CUDA Core
category: compute
examples:
- 16,384 CUDA cores in the GeForce RTX 4090
- 10,496 CUDA cores in the GeForce RTX 3090
- AMD spec sheets count Stream Processors (6,144 on Radeon RX 7900 XTX)
- Intel counts Xe Vector Engines (XVE), 16 per Xe-core
related:
- glossary-term/tensor-core
- glossary-term/tflops
tags:
- compute
- cuda
- shader
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/
  title: GeForce RTX 4090 specifications (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/30-series/rtx-3090-3090ti/
  title: GeForce RTX 3090 specifications (NVIDIA)
  trust: 0.95
- url: https://www.amd.com/en/products/graphics/desktops/radeon/7000-series/amd-radeon-rx-7900xtx.html
  title: Radeon RX 7900 XTX specifications (AMD)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/developer/articles/technical/introduction-to-the-xe-hpg-architecture.html
  title: Introduction to the Xe-HPG Architecture (Intel)
  trust: 0.95
- url: https://developer.nvidia.com/blog/nvidia-turing-architecture-in-depth/
  title: NVIDIA Turing Architecture In-Depth (NVIDIA)
  trust: 0.95
---

## Definition

CUDA cores are the cores NVIDIA counts as "NVIDIA CUDA Cores" on its GPU specification sheets. Other
makers count their own units: AMD lists Stream Processors, and Intel lists Xe Vector Engines (XVE),
which Intel describes as the sub-block that executes instructions.

## Why You Care

The matrix operations at the core of deep learning run on separate units, which NVIDIA calls Tensor
Cores and counts on a separate line. A CUDA-core count alone does not describe a GPU's AI throughput.
