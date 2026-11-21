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
updated: '2026-11-21'
sources:
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html", title: "AMD Instinct MI300X Accelerators (AMD)", trust: 0.95 }
---

## Definition
TFLOPS is trillions (10^12) of floating-point operations per second; TOPS counts integer operations,
for example INT8. Makers publish peak theoretical figures, each at a stated precision.

## Why You Care
A figure means little without its precision and its dense or sparse basis. AMD lists the Instinct MI300X
at 163.4 TFLOPs peak FP32, 1.3 PFLOPs peak FP16, 2.61 PFLOPs peak FP8 and 5.22 PFLOPs FP8 with
structured sparsity. Compare like with like, and treat any peak as a ceiling, not a measured speed.
