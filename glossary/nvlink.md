---
id: glossary-term/nvlink
type: glossary-term
slug: nvlink
schema_version: 3.0
title: NVLink
term: NVLink
category: interconnect
examples:
- NVLink on Tesla P100 (up to four links)
- Fourth-generation NVLink on H100 SXM (900 GB/s)
- Fifth-generation NVLink on Blackwell (1,800 GB/s per GPU)
related:
- glossary-term/nvswitch
- glossary-term/pcie
tags:
- interconnect
- nvlink
- scale-out
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/en-us/data-center/nvlink/
  title: NVIDIA NVLink (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/blog/inside-pascal/
  title: 'Inside Pascal: NVIDIA''s Newest Computing Platform (NVIDIA)'
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU (NVIDIA)
  trust: 0.95
---

## Definition

NVLink is NVIDIA's direct GPU-to-GPU interconnect. Per-GPU bandwidth is 900 GB/s for the fourth
generation (Hopper), 1,800 GB/s for the fifth (Blackwell) and 3,000 GB/s for the sixth (Vera Rubin,
preliminary), as NVIDIA's NVLink page lists them.

## Why You Care

A model too large for one GPU is split across several, which then exchange data constantly. For
comparison, NVIDIA lists H100 SXM at 900 GB/s over NVLink and 128 GB/s over PCIe Gen5.
