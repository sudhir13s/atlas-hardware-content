---
id: gpu-architecture/gcn
type: gpu-architecture
slug: gcn
schema_version: 1.0
title: "AMD GCN (Graphics Core Next)"
name: "Graphics Core Next"
vendor: AMD
codename: "GCN 1–5 (Southern Islands → Vega)"
year: 2012
successor: gpu-architecture/rdna
process_node: "TSMC 28nm (early) → GlobalFoundries/TSMC 14nm (Vega)"
segment: "consumer + datacenter"
representative_gpus: ["Radeon HD 7970 (2012)", "Radeon R9 290X (2013)", "Radeon RX Vega 64 (2017)", "Radeon Instinct MI25 (2017)"]
key_innovation: "A compute-first architecture built on scalar plus SIMD vector units, making AMD GPUs strong general-purpose compute engines."
innovations: ["Scalar + SIMD vector compute units", "Asynchronous Compute Engines", "HBM/HBM2 on Fiji and Vega", "Rapid Packed Math (packed FP16) on Vega", "Infinity Fabric debut (Vega)"]
precision_support: ["FP64", "FP32", "FP16 (Vega)"]
memory_tech: "GDDR5 → HBM2 (Vega)"
interconnect: "PCIe 3.0 / Infinity Fabric (Vega)"
tags: [amd, gcn, vega, compute, hbm2]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Graphics_Core_Next", title: "Graphics Core Next — Wikipedia", trust: 0.8 }
  - { url: "https://www.amd.com/system/files/documents/rdna-whitepaper.pdf", title: "AMD RDNA Architecture Whitepaper (GCN background)", trust: 0.9 }
---

## What Changed
Graphics Core Next was AMD's long-lived (2012–2019, five revisions) **compute-first** architecture. It
paired each SIMD vector unit with a **scalar unit** and exposed **Asynchronous Compute Engines**,
making GCN GPUs unusually capable at general-purpose compute for their era — a reason they were popular
for cryptocurrency mining and OpenCL workloads. Later GCN generations added the technologies AMD would
carry into its AI accelerators: **HBM** stacked memory (Fiji, then HBM2 on Vega), **Rapid Packed Math**
for double-rate FP16 (Vega), and the first use of **Infinity Fabric** on-package. The Radeon Instinct
MI25 (Vega) was AMD's early datacenter deep-learning card. GCN eventually split into two successors:
**RDNA** for gaming efficiency and **CDNA** for pure datacenter compute.
