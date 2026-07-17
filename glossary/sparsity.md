---
id: glossary-term/sparsity
type: glossary-term
slug: sparsity
schema_version: 1.0
title: "Structured Sparsity"
term: "Structured Sparsity"
category: compute
examples: ["2:4 structured sparsity on Ampere Tensor Cores", "Up to 2x throughput on sparsified weights"]
related: [glossary-term/tensor-core, glossary-term/fp8]
tags: [compute, sparsity, tensor-core]
updated: 2026-07-17
sources:
  - { url: "https://developer.nvidia.com/blog/accelerating-inference-with-sparsity-using-ampere-and-tensorrt/", title: "Accelerating Inference with Sparsity (NVIDIA)", trust: 0.9 }
---

## Definition
Structured sparsity is a hardware-friendly way to skip zero-valued weights. NVIDIA's 2:4 scheme (from
Ampere onward) requires that in every group of four weights, two are zero; the Tensor Core then processes
only the nonzero pair, plus a small index, in roughly half the work.

## Why You Care
Pruning a network to 2:4 sparsity can nearly double Tensor-Core throughput and cut memory for the sparse
weights — but only if the model is pruned into exactly that pattern and fine-tuned to recover accuracy.
It is a real speedup for inference when you control the model, and it explains why a spec sheet often
lists two Tensor-Core numbers: dense and (2x) sparse.
