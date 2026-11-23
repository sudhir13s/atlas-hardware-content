---
id: glossary-term/sparsity
type: glossary-term
slug: sparsity
schema_version: 3.0
title: Structured Sparsity
term: Structured Sparsity
category: compute
examples:
- 2:4 structured sparsity on A100 Tensor Cores
- 'Instinct MI300X: 2.61 PFLOPs peak FP8, 5.22 PFLOPs with structured sparsity'
related:
- glossary-term/tensor-core
- glossary-term/fp8
tags:
- compute
- sparsity
- tensor-core
updated: '2026-11-21'
sources:
- url: https://developer.nvidia.com/blog/accelerating-inference-with-sparsity-using-ampere-and-tensorrt/
  title: Accelerating Inference with Sparsity Using the NVIDIA Ampere Architecture and NVIDIA TensorRT (NVIDIA)
  trust: 0.95
- url: https://developer.nvidia.com/blog/nvidia-ampere-architecture-in-depth/
  title: NVIDIA Ampere Architecture In-Depth (NVIDIA)
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html
  title: AMD Instinct MI300X Accelerators (AMD)
  trust: 0.95
---

## Definition

Structured sparsity is a fixed pattern of zero weights the hardware can skip. In NVIDIA's 2:4 pattern,
added to Tensor Cores with the A100, two of every four contiguous values are zero. The matrix is stored
at half size plus metadata marking the nonzero positions.

## Why You Care

NVIDIA states that at 2:4 sparsity the Tensor Cores complete the same effective calculation in half
the time, but the pruned model must be retrained to recover accuracy. This is why spec sheets list two
figures, dense and "with structured sparsity".
