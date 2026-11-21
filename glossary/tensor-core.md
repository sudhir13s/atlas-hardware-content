---
id: glossary-term/tensor-core
type: glossary-term
slug: tensor-core
schema_version: 1.0
title: "Tensor Core"
term: "Tensor Core"
category: compute
examples: ["Tensor Cores introduced with Volta (V100)", "4th-generation Tensor Cores with FP8 in Hopper (H100)", "AMD's counterpart: Matrix Cores (1,216 on Instinct MI300X)", "Intel's counterpart: XMX engines"]
related: [glossary-term/cuda-core, glossary-term/tflops, glossary-term/bf16]
tags: [compute, tensor-core, matrix]
updated: '2026-11-21'
sources:
  - { url: "https://developer.nvidia.com/blog/programming-tensor-cores-cuda-9/", title: "Programming Tensor Cores in CUDA 9 (NVIDIA)", trust: 0.95 }
  - { url: "https://developer.nvidia.com/blog/nvidia-turing-architecture-in-depth/", title: "NVIDIA Turing Architecture In-Depth (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/h100/", title: "NVIDIA H100 Tensor Core GPU (NVIDIA)", trust: 0.95 }
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html", title: "AMD Instinct MI300X Accelerators (AMD)", trust: 0.95 }
  - { url: "https://www.intel.com/content/www/us/en/developer/articles/technical/introduction-to-the-xe-hpg-architecture.html", title: "Introduction to the Xe-HPG Architecture (Intel)", trust: 0.95 }
---

## Definition
A Tensor Core is an NVIDIA unit for matrix math. On Volta, where Tensor Cores first appeared, each one
performs D = A × B + C on 4×4 matrices with FP16 inputs and FP32 accumulation. AMD's counterpart is the
Matrix Core; Intel's is the XMX (Xe Matrix Extensions) engine.

## Why You Care
NVIDIA describes Tensor Cores as execution units built for the matrix operations at the core of deep
learning training and inference. Their throughput is quoted per precision (FP16, FP8, INT8 and so on),
so check which precision a figure uses.
