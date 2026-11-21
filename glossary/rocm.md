---
id: glossary-term/rocm
type: glossary-term
slug: rocm
schema_version: 1.0
title: "ROCm"
term: "ROCm"
category: software
examples: ["HIP: AMD's C++ runtime API and kernel language", "HIPIFY: tools that translate CUDA API calls to HIP", "PyTorch on ROCm"]
related: []
tags: [software, rocm, amd]
updated: '2026-11-21'
sources:
  - { url: "https://rocm.docs.amd.com/en/latest/what-is-rocm.html", title: "What is ROCm? (AMD ROCm documentation)", trust: 0.95 }
  - { url: "https://rocm.docs.amd.com/projects/HIP/en/latest/what_is_hip.html", title: "What is HIP? (AMD ROCm documentation)", trust: 0.95 }
---

## Definition
ROCm is AMD's open software stack for GPU computing: runtimes, compilers, system utilities, and math
and compute libraries. Its programming model, HIP, is a C++ runtime API and kernel language for AMD GPUs.

## Why You Care
Hardware is only usable through its software. AMD states that HIP is not a drop-in replacement for
CUDA, so porting CUDA code usually needs manual work and tuning; check ROCm support for your framework
and workload before choosing AMD hardware.
