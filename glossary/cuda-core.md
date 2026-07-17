---
id: glossary-term/cuda-core
type: glossary-term
slug: cuda-core
schema_version: 1.0
title: "CUDA Core"
term: "CUDA Core"
category: compute
examples: ["16,384 CUDA cores in the RTX 4090", "AMD's equivalent: Stream Processors", "Intel's equivalent: Vector Engines"]
related: [glossary-term/tensor-core, glossary-term/tflops]
tags: [compute, cuda, shader]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/CUDA", title: "CUDA — Wikipedia", trust: 0.8 }
---

## Definition
A CUDA core is a general-purpose scalar arithmetic lane on an NVIDIA GPU — the basic unit that executes
floating-point and integer operations for shaders and compute kernels. AMD calls the equivalent a Stream
Processor; Intel calls it a Vector Engine lane.

## Why You Care
CUDA-core count and clock give a GPU's general FP32 throughput, which matters for graphics and
non-matrix compute. For AI specifically, CUDA cores handle the "everything else" around the matrix math
(activations, normalization, elementwise ops), while Tensor Cores handle the heavy matrix multiplies.
Comparing CUDA-core counts across different architectures is misleading because per-core efficiency
changes every generation.
