---
id: gpu-architecture/cdna-2
type: gpu-architecture
slug: cdna-2
schema_version: 1.0
title: "AMD CDNA 2"
name: "CDNA 2"
vendor: AMD
codename: "Aldebaran"
year: 2021
predecessor: gpu-architecture/cdna
successor: gpu-architecture/cdna-3
process_node: "TSMC 6nm"
segment: "datacenter"
representative_gpus: ["Instinct MI250X (2021)", "Instinct MI250 (2021)", "Instinct MI210 (2022)"]
key_innovation: "A multi-die datacenter GPU: two compute dies linked by Infinity Fabric, with full-rate FP64 matrix operations for exascale HPC."
innovations: ["Dual-die multi-chip module (2 compute dies as one accelerator)", "Full-rate FP64 matrix operations", "Infinity Fabric 3.0", "Coherent CPU–GPU link with EPYC", "Powers the Frontier exascale supercomputer"]
precision_support: ["FP64", "FP32", "FP16", "BF16", "INT8"]
memory_tech: "HBM2e"
interconnect: "Infinity Fabric 3.0, PCIe 4.0"
tags: [amd, cdna-2, mi250x, fp64, exascale]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/CDNA_(microarchitecture)#CDNA_2", title: "CDNA 2 — Wikipedia", trust: 0.8 }
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi200/mi250x.html", title: "AMD Instinct MI250X Accelerator", trust: 0.9 }
---

## What Changed
CDNA 2 scaled the datacenter line by going **multi-die**: the Instinct MI250X packages **two compute
dies** on one module, linked by **Infinity Fabric 3.0** and presented together to fill an OAM socket.
It emphasized **full-rate FP64 matrix operations**, making it exceptionally strong for double-precision
HPC — CDNA 2 powers **Frontier**, the first machine to break the exascale barrier. A **coherent
Infinity Fabric link to AMD EPYC CPUs** let the CPU and GPU share a memory view, foreshadowing the
tighter integration of CDNA 3. With **HBM2e** and the dual-die approach, CDNA 2 was AMD's first
accelerator to genuinely rival NVIDIA's top HPC parts, even as NVIDIA's Tensor-Core AI throughput
still led on lower precisions.
