---
id: glossary-term/rocm
type: glossary-term
slug: rocm
schema_version: 1.0
title: "ROCm"
term: "ROCm"
category: software
examples: ["ROCm on Instinct MI250X / MI300X", "HIP: AMD's CUDA-like C++ dialect", "PyTorch and vLLM support on ROCm"]
related: []
tags: [software, rocm, amd]
updated: 2026-07-17
sources:
  - { url: "https://rocm.docs.amd.com/", title: "AMD ROCm Documentation", trust: 0.9 }
---

## Definition
ROCm (Radeon Open Compute) is AMD's open-source GPU-compute software stack — drivers, libraries, and the
HIP programming model — the counterpart to NVIDIA's CUDA. HIP code can often be compiled to run on both
AMD and NVIDIA GPUs.

## Why You Care
Hardware is only as useful as its software. NVIDIA's dominance rests heavily on CUDA's maturity; AMD's
competitiveness in AI depends on ROCm supporting the frameworks people actually use (PyTorch, vLLM,
Triton) well enough to run models without heroics. When comparing an MI300X to an H100, ROCm's maturity
for your specific workload is often the deciding factor, not the raw specs.
