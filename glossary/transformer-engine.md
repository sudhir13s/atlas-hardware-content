---
id: glossary-term/transformer-engine
type: glossary-term
slug: transformer-engine
schema_version: 1.0
title: "Transformer Engine"
term: "Transformer Engine"
category: compute
examples: ["1st-gen Transformer Engine on Hopper (FP8)", "2nd-gen on Blackwell (FP4/FP6)"]
related: [glossary-term/fp8, glossary-term/tensor-core]
tags: [compute, transformer-engine, fp8]
updated: 2026-07-17
sources:
  - { url: "https://docs.nvidia.com/deeplearning/transformer-engine/", title: "NVIDIA Transformer Engine Documentation", trust: 0.9 }
---

## Definition
The Transformer Engine is a combination of hardware (Tensor Cores that support FP8, and on Blackwell
FP4/FP6) and a software library that tracks per-tensor statistics during training and inference to choose
the lowest precision that preserves accuracy, rescaling values as needed.

## Why You Care
Low-precision formats like FP8 are fast but numerically fragile; naively casting a transformer to FP8
usually diverges. The Transformer Engine automates the scaling and precision decisions that make FP8
usable, which is why Hopper could advertise ~2x transformer throughput over BF16. It is the practical
bridge between raw low-precision hardware and models that still converge.
