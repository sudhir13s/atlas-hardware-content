---
id: glossary-term/fp8
type: glossary-term
slug: fp8
schema_version: 3.0
title: FP8 (8-bit Floating Point)
term: FP8 (8-bit Floating Point)
category: precision
examples:
- E4M3 and E5M2 on H100 (Hopper)
- FP8 Transformer Engine on Ada Lovelace
- FP8 (E5M2, E4M3) on Instinct MI300X
- FP6 and FP4 on Blackwell Tensor Cores
related:
- glossary-term/bf16
- glossary-term/sparsity
- glossary-term/transformer-engine
tags:
- precision
- fp8
- low-precision
updated: '2026-11-21'
sources:
- url: https://arxiv.org/abs/2209.05433
  title: FP8 Formats for Deep Learning (Micikevicius et al.)
  trust: 0.95
- url: https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/
  title: NVIDIA Hopper Architecture In-Depth (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/ada-lovelace-architecture/
  title: NVIDIA Ada Lovelace Architecture (NVIDIA)
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html
  title: AMD Instinct MI300X Accelerators (AMD)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/tensor-cores/
  title: NVIDIA Tensor Cores (NVIDIA)
  trust: 0.95
---

## Definition

FP8 is an 8-bit floating-point format proposed for deep learning in two encodings: E4M3 (4 exponent
bits, 3 mantissa bits) and E5M2 (5 exponent bits, 2 mantissa bits). NVIDIA describes E4M3 as favouring
precision and E5M2 as favouring dynamic range. Each value takes half the bits of FP16 or BF16.

## Why You Care

Half the bits means half the memory per value, and makers rate FP8 above 16-bit math: AMD lists 2.61
PFLOPs peak FP8 against 1.3 PFLOPs peak FP16 for the Instinct MI300X. The FP8 paper reports matching
16-bit training quality across image and language tasks; NVIDIA's Transformer Engine manages the scaling.
