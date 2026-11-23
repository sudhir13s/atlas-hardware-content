---
id: upgrade-path/nvidia-datacenter
type: upgrade-path
slug: nvidia-datacenter
schema_version: 3.0
title: NVIDIA datacenter training GPUs
vendor: NVIDIA
family: Datacenter (Tesla / Data Center)
steps:
- gpu_name: Tesla V100
  architecture_id: gpu-architecture/volta
  year: 2017
- gpu_name: A100
  architecture_id: gpu-architecture/ampere
  year: 2020
- gpu_name: H100
  architecture_id: gpu-architecture/hopper
  year: 2022
- gpu_id: gpu/nvidia-h200
  architecture_id: gpu-architecture/hopper
  year: 2023
- gpu_id: gpu/nvidia-b200
  architecture_id: gpu-architecture/blackwell
  year: 2024
tags:
- nvidia
- datacenter
- training
updated: '2026-11-21'
sources:
- url: https://nvidianews.nvidia.com/news/nvidia-launches-revolutionary-volta-gpu-platform-fueling-next-era-of-ai-and-high-performance-computing
  title: NVIDIA — Tesla V100 announcement (10 May 2017)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidias-new-ampere-data-center-gpu-in-full-production
  title: NVIDIA — A100 announcement (14 May 2020)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-announces-hopper-architecture-the-next-generation-of-accelerated-computing
  title: NVIDIA — Hopper and H100 announcement (22 March 2022)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-supercharges-hopper-the-worlds-leading-ai-computing-platform
  title: NVIDIA — H200 announcement (13 November 2023)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-blackwell-platform-arrives-to-power-a-new-era-of-computing
  title: NVIDIA — Blackwell platform announcement (18 March 2024)
  trust: 0.95
---

## Overview

NVIDIA's data center GPUs by announcement year. Memory moved from **HBM2** (Tesla V100) to **HBM3**
(H100) and **HBM3e** (H200). NVIDIA's announcements name **TF32** for the A100, **FP8** for the H100,
and **4-bit floating point (FP4)** inference in Blackwell's second-generation Transformer Engine.
