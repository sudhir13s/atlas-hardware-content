---
id: gpu-architecture/cdna
type: gpu-architecture
slug: cdna
schema_version: 1.0
title: "AMD CDNA"
name: "CDNA"
vendor: AMD
codename: "Arcturus"
year: 2020
predecessor: gpu-architecture/gcn
successor: gpu-architecture/cdna-2
process_node: "TSMC 7nm"
segment: "datacenter"
representative_gpus: ["Instinct MI100 (2020)"]
key_innovation: "AMD's first compute-only datacenter architecture, introducing Matrix Cores for AI and HPC while removing the graphics pipeline entirely."
innovations: ["Matrix Cores (MFMA matrix instructions)", "Compute-only design (no graphics/display hardware)", "Infinity Fabric for GPU-to-GPU links", "Full-rate FP64 for HPC"]
precision_support: ["FP64", "FP32", "FP16", "BF16", "INT8"]
memory_tech: "HBM2"
interconnect: "Infinity Fabric, PCIe 4.0"
tags: [amd, cdna, mi100, matrix-cores, datacenter]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/CDNA_(microarchitecture)", title: "CDNA (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi100.html", title: "AMD Instinct MI100 Accelerator", trust: 0.9 }
---

## What Changed
CDNA (Compute DNA) split AMD's GPU lineage in two: where RDNA optimized for gaming, CDNA was a
**compute-only datacenter architecture** with the graphics and display hardware stripped out entirely.
Its key addition was **Matrix Cores**, executing MFMA (matrix fused multiply-add) instructions — AMD's
answer to NVIDIA's Tensor Cores — accelerating the dense matrix math of AI and HPC. The Instinct MI100
was the first CDNA part, combining Matrix Cores, strong **full-rate FP64** for scientific computing,
**HBM2** memory, and **Infinity Fabric** links between GPUs. CDNA gave AMD a credible datacenter
accelerator line for the first time and established the software (ROCm) and hardware direction that
CDNA 2 and CDNA 3 would scale up toward competing with NVIDIA at the top of the market.
