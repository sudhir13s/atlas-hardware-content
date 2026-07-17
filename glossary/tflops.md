---
id: glossary-term/tflops
type: glossary-term
slug: tflops
schema_version: 1.0
title: "TFLOPS / TOPS"
term: "TFLOPS / TOPS"
category: compute
examples: ["FP32 TFLOPS for general compute", "FP16/BF16 Tensor TFLOPS for AI", "INT8 TOPS for inference"]
related: [glossary-term/tensor-core, glossary-term/bf16]
tags: [compute, tflops, benchmark]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/FLOPS", title: "FLOPS — Wikipedia", trust: 0.8 }
---

## Definition
TFLOPS is trillions (10^12) of floating-point operations per second; TOPS is the same for integer
operations. It is a peak theoretical throughput derived from core count × clock × ops-per-core, always
quoted at a specific precision (FP64, FP32, TF32, BF16, FP16, FP8, INT8).

## Why You Care
A TFLOPS number is meaningless without its precision and its dense/sparse basis — an "AI TFLOPS" figure at
FP8 with sparsity can be 16x the FP32 figure for the same chip. It is also a peak the hardware rarely
reaches; real utilization depends on memory bandwidth, kernel quality, and batch size. Use it to compare
like-for-like, never as a standalone performance promise.
