---
id: glossary-term/fp8
type: glossary-term
slug: fp8
schema_version: 1.0
title: "FP8 (8-bit Floating Point)"
term: "FP8 (8-bit Floating Point)"
category: precision
examples: ["FP8 (E4M3 / E5M2) on Hopper Transformer Engine", "FP8 on Ada, MI300X, Gaudi 3", "Successor formats FP6/FP4 on Blackwell"]
related: [glossary-term/bf16, glossary-term/sparsity, glossary-term/transformer-engine]
tags: [precision, fp8, low-precision]
updated: 2026-07-17
sources:
  - { url: "https://arxiv.org/abs/2209.05433", title: "FP8 Formats for Deep Learning (Micikevicius et al.)", trust: 0.9 }
---

## Definition
FP8 is an 8-bit floating-point format for neural networks, standardized in two variants: E4M3 (4 exponent,
3 mantissa bits — more precision, less range) and E5M2 (5 exponent, 2 mantissa — more range, less
precision). It halves the bits of FP16/BF16.

## Why You Care
Fewer bits per value means more values moved per second and more math per clock, so FP8 roughly doubles
throughput and halves memory footprint versus 16-bit — a major speedup for training and inference. The
catch is accuracy: FP8's tiny range/precision requires careful scaling (e.g. Hopper's Transformer Engine)
to avoid overflow/underflow. FP8 support is now a headline feature distinguishing recent accelerators.
