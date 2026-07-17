---
id: gpu-architecture/ampere
type: gpu-architecture
slug: ampere
schema_version: 1.0
title: "NVIDIA Ampere"
name: "Ampere"
vendor: NVIDIA
codename: "GA100 / GA10x"
year: 2020
predecessor: gpu-architecture/turing
successor: gpu-architecture/hopper
process_node: "TSMC 7N (A100) / Samsung 8N (GeForce)"
segment: "consumer + datacenter"
representative_gpus: ["A100 (2020)", "GeForce RTX 3090 (2020)", "GeForce RTX 3080 (2020)", "A40 (2020)"]
key_innovation: "Third-generation Tensor Cores added TF32, BF16, and 2:4 structured sparsity, and the A100 introduced Multi-Instance GPU (MIG) partitioning."
innovations: ["3rd-generation Tensor Cores", "TF32 math format (drop-in FP32 range, Tensor-Core speed)", "BF16 support", "2:4 structured sparsity acceleration", "Multi-Instance GPU (MIG)", "NVLink 3.0"]
precision_support: ["FP64", "TF32", "BF16", "FP16", "INT8", "INT4"]
memory_tech: "HBM2e (A100) / GDDR6X (GeForce)"
interconnect: "NVLink 3.0 / PCIe 4.0"
tags: [nvidia, ampere, a100, tf32, bf16, sparsity, mig]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Ampere_(microarchitecture)", title: "Ampere (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://images.nvidia.com/aem-dam/en-zz/Solutions/data-center/nvidia-ampere-architecture-whitepaper.pdf", title: "NVIDIA A100 Ampere Architecture Whitepaper", trust: 0.95 }
---

## What Changed
Ampere's A100 became the defining training GPU of the early LLM boom. Its **third-generation Tensor
Cores** introduced **TF32** — a format with FP32's dynamic range but reduced mantissa, giving
Tensor-Core speed as a near drop-in for FP32 training — plus native **BF16** and hardware acceleration
for **2:4 structured sparsity** (skipping half the weights in a fixed pattern). The A100 also added
**Multi-Instance GPU (MIG)**, letting one physical GPU be partitioned into up to seven isolated
instances so smaller jobs need not waste a whole card. On the consumer side, Ampere GeForce (RTX 30
series) paired a Samsung 8nm process with **GDDR6X** memory. Ampere is where the datacenter feature set
(TF32, BF16, sparsity, MIG, HBM2e, NVLink 3.0) pulled decisively ahead of the gaming line.
