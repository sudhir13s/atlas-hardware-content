---
id: glossary-term/transformer-engine
type: glossary-term
slug: transformer-engine
schema_version: 3.0
title: Transformer Engine
term: Transformer Engine
category: compute
examples:
- Transformer Engine with FP8 on Hopper (H100)
- Second-generation Transformer Engine with FP4 on Blackwell
related:
- glossary-term/fp8
- glossary-term/tensor-core
tags:
- compute
- transformer-engine
- fp8
updated: '2026-11-21'
sources:
- url: https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/
  title: NVIDIA Hopper Architecture In-Depth (NVIDIA)
  trust: 0.95
- url: https://docs.nvidia.com/deeplearning/transformer-engine/
  title: NVIDIA Transformer Engine Documentation (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/tensor-cores/
  title: NVIDIA Tensor Cores (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/ada-lovelace-architecture/
  title: NVIDIA Ada Lovelace Architecture (NVIDIA)
  trust: 0.95
---

## Definition

The Transformer Engine is NVIDIA's combination of Tensor Core hardware and a software library. On Hopper,
NVIDIA states it analyses the statistics of Tensor Core outputs, chooses between FP8 and 16-bit math
per layer, and rescales tensor data into the representable range.

## Why You Care

FP8 is fast but has little range; the Transformer Engine library manages the scaling factors and
quantization metadata that low-precision training needs. NVIDIA's library supports FP8 on Hopper, Ada,
Blackwell and Rubin, and MXFP8 and NVFP4 on Blackwell.
