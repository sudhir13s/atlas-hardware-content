---
id: glossary-term/hbm
type: glossary-term
slug: hbm
schema_version: 3.0
title: HBM (High Bandwidth Memory)
term: HBM (High Bandwidth Memory)
category: memory
examples:
- HBM2 on Tesla P100
- HBM3 on H100 SXM
- 141 GB HBM3e on H200
- 192 GB HBM3 on Instinct MI300X
related:
- glossary-term/gddr6
- glossary-term/memory-bandwidth
- glossary-term/vram
tags:
- memory
- hbm
- bandwidth
updated: '2026-11-21'
sources:
- url: https://developer.nvidia.com/blog/inside-pascal/
  title: 'Inside Pascal: NVIDIA''s Newest Computing Platform (NVIDIA)'
  trust: 0.95
- url: https://www.jedec.org/news/pressreleases/jedec-publishes-hbm3-update-high-bandwidth-memory-hbm-standard
  title: JEDEC Publishes HBM3 Update to High Bandwidth Memory (HBM) Standard (JEDEC)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/
  title: NVIDIA Hopper Architecture In-Depth (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/
  title: 'Mastering LLM Techniques: Inference Optimization (NVIDIA)'
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h200/
  title: NVIDIA H200 Tensor Core GPU (NVIDIA)
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html
  title: AMD Instinct MI300X Accelerators (AMD)
  trust: 0.95
---

## Definition

HBM is memory built from vertical stacks of DRAM dies, placed beside the GPU and connected through a
silicon interposer (NVIDIA, Tesla P100). JEDEC's HBM3 standard defines up to 6.4 Gb/s per pin, or
819 GB/s per device. Generations shipped on the products here are HBM2, HBM3 and HBM3e.

## Why You Care

NVIDIA states that large-language-model inference is frequently memory-bandwidth bound, and HBM is the
memory datacenter accelerators use for TB/s bandwidth: 3.35 TB/s on H100 SXM, 4.8 TB/s on H200. HBM
capacity also sets how large a model fits on one device.
