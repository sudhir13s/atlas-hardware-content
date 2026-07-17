---
id: glossary-term/tensor-core
type: glossary-term
slug: tensor-core
schema_version: 1.0
title: "Tensor Core"
term: "Tensor Core"
category: compute
examples: ["1st-gen Tensor Cores in Volta (V100)", "4th-gen FP8 Tensor Cores in Hopper (H100)", "AMD's equivalent: Matrix Cores"]
related: [glossary-term/cuda-core, glossary-term/tflops, glossary-term/bf16]
tags: [compute, tensor-core, matrix]
updated: 2026-07-17
sources:
  - { url: "https://www.nvidia.com/en-us/data-center/tensor-cores/", title: "NVIDIA Tensor Cores", trust: 0.9 }
---

## Definition
A Tensor Core is a specialized hardware unit that computes a small matrix multiply-accumulate
(D = A × B + C) in a single operation, typically with reduced-precision inputs (FP16/BF16/FP8) and
higher-precision accumulation (FP32). NVIDIA introduced them in Volta; AMD's equivalent is the Matrix
Core, Intel's is the XMX engine.

## Why You Care
Neural-network training and inference are dominated by matrix multiplication. Tensor Cores do that math
far faster than general-purpose CUDA cores, so a GPU's Tensor-Core throughput (not its raw FP32 rate) is
the number that best predicts AI performance. When a vendor quotes a huge "AI TFLOPS" or "TOPS" figure,
it is almost always a Tensor/Matrix-Core number at low precision.
