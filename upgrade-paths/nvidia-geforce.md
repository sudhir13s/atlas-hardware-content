---
id: upgrade-path/nvidia-geforce
type: upgrade-path
slug: nvidia-geforce
schema_version: 1.0
title: "NVIDIA GeForce flagship consumer GPUs"
vendor: NVIDIA
family: "GeForce (consumer)"
steps:
  - { gpu_id: "GeForce GTX 1080 Ti", architecture_id: gpu-architecture/pascal, year: 2017 }
  - { gpu_id: "GeForce RTX 2080 Ti", architecture_id: gpu-architecture/turing, year: 2018 }
  - { gpu_id: "GeForce RTX 3090", architecture_id: gpu-architecture/ampere, year: 2020 }
  - { gpu_id: "GeForce RTX 4090", architecture_id: gpu-architecture/ada-lovelace, year: 2022 }
  - { gpu_id: "GeForce RTX 5090", architecture_id: gpu-architecture/blackwell, year: 2025 }
tags: [nvidia, geforce, consumer]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/GeForce", title: "GeForce — Wikipedia", trust: 0.8 }
---

## Overview
The consumer GeForce flagship line, generation by generation. The Turing step introduced RT and Tensor
Cores to consumers; later steps grew VRAM (11 GB → 24 GB → 32 GB) and added FP8, making high-end GeForce
cards popular for local AI fine-tuning and inference.
