---
id: gpu-architecture/cdna-3
type: gpu-architecture
slug: cdna-3
schema_version: 1.0
title: "AMD CDNA 3"
name: "CDNA 3"
vendor: AMD
codename: "Aqua Vanjaram (MI300)"
year: 2023
predecessor: gpu-architecture/cdna-2
process_node: "TSMC 5nm + 6nm"
segment: "datacenter"
representative_gpus: ["Instinct MI300X (2023)", "Instinct MI300A APU (2023)", "Instinct MI325X (2024)"]
key_innovation: "A 3D-stacked chiplet accelerator with 192 GB of HBM3, and an APU variant (MI300A) fusing Zen 4 CPU cores and CDNA 3 GPU on one package with unified memory."
innovations: ["3D die stacking (compute chiplets on base dies)", "MI300A APU (Zen 4 CPU + CDNA 3 GPU, unified memory)", "192 GB HBM3 on MI300X", "Unified memory architecture", "FP8 support", "Infinity Fabric 4.0"]
precision_support: ["FP64", "FP32", "FP16", "BF16", "FP8", "INT8"]
memory_tech: "HBM3"
interconnect: "Infinity Fabric 4.0, PCIe 5.0"
tags: [amd, cdna-3, mi300x, mi300a, hbm3, fp8, apu]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/CDNA_(microarchitecture)#CDNA_3", title: "CDNA 3 — Wikipedia", trust: 0.8 }
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html", title: "AMD Instinct MI300X Accelerator", trust: 0.9 }
---

## What Changed
CDNA 3 is AMD's most direct challenge to NVIDIA in AI. The MI300 family uses **3D die stacking** —
compute chiplets mounted on top of base dies over silicon interposers — to pack enormous compute and
memory into one package. The **MI300X** ships with **192 GB of HBM3**, well above an H100's memory, a
deliberate advantage for large-model inference where model weights and KV cache must fit on-device. The
**MI300A** is an **APU**: it replaces some GPU chiplets with **Zen 4 CPU** cores so CPU and GPU share
one **unified HBM memory** pool, eliminating host-device copies — it powers the El Capitan
supercomputer. CDNA 3 adds **FP8** for low-precision AI. Paired with a maturing **ROCm** software
stack, MI300X made AMD a serious second source for datacenter AI compute for the first time.
