---
id: guide/memory-bandwidth
type: guide
slug: memory-bandwidth
schema_version: 3.0
title: 'Memory bandwidth: why speed matters'
page_section: background
order: 4
points:
- name: HBM3e
  text: 4.8 TB/s on the NVIDIA H200; 6 TB/s peak on the AMD Instinct MI325X.
- name: HBM3
  text: 3.35 TB/s on the NVIDIA H100 SXM; 5.3 TB/s peak on the AMD Instinct MI300X.
- name: GDDR6 and GDDR7
  text: 864 GB/s on the NVIDIA L40S (GDDR6); 1,792 GB/s on the NVIDIA RTX PRO 6000 Blackwell Workstation Edition (GDDR7).
- name: Apple unified memory
  text: 614 GB/s on the M5 Max with 40-core GPU; 800 GB/s on the M1 Ultra. CPU and GPU share the memory, so data is not copied between them.
tags:
- gpu-buying-guide
- memory-bandwidth
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/en-us/data-center/h200/
  title: NVIDIA H200 Tensor Core GPU
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi325x.html
  title: AMD Instinct MI325X Accelerators
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html
  title: AMD Instinct MI300X Accelerators
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/l40s/
  title: NVIDIA L40S GPU
  trust: 0.95
- url: https://www.nvidia.com/en-us/products/workstations/professional-desktop-gpus/rtx-pro-6000/
  title: NVIDIA RTX PRO 6000 Blackwell Workstation Edition
  trust: 0.95
- url: https://www.apple.com/macbook-pro/specs/
  title: MacBook Pro - Technical Specifications (Apple)
  trust: 0.95
- url: https://www.apple.com/newsroom/2022/03/apple-unveils-m1-ultra-the-worlds-most-powerful-chip-for-a-personal-computer/
  title: Apple unveils M1 Ultra (Apple Newsroom)
  trust: 0.95
- url: https://github.com/ml-explore/mlx
  title: 'MLX: an array framework for Apple silicon'
  trust: 0.9
- url: https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/
  title: 'Mastering LLM Techniques: Inference Optimization (NVIDIA Technical Blog)'
  trust: 0.95
---

## Overview

NVIDIA notes that **token generation** (the decode phase of large language model inference) is **memory-bound**: moving weights from memory dominates the time. Higher bandwidth means faster token generation.

## Takeaway

**Estimate (upper bound):** tokens per second ≤ bandwidth ÷ bytes read per token, assuming one request at a time, each weight read once per token, and no KV cache or overhead. A 7B model at 16-bit is about 14 GB (NVIDIA), so the H100 SXM's 3,350 GB/s gives 3,350 ÷ 14 ≈ 240 tokens per second at most.
