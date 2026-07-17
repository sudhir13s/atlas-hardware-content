---
id: gpu-architecture/rdna
type: gpu-architecture
slug: rdna
schema_version: 1.0
title: "AMD RDNA"
name: "RDNA"
vendor: AMD
codename: "Navi 1x"
year: 2019
predecessor: gpu-architecture/gcn
successor: gpu-architecture/rdna-2
process_node: "TSMC 7nm"
segment: "consumer"
representative_gpus: ["Radeon RX 5700 XT (2019)", "Radeon RX 5700 (2019)", "Radeon RX 5500 XT (2019)"]
key_innovation: "A ground-up redesign of the compute unit for gaming, prioritizing performance-per-clock and per-watt over GCN's raw compute width."
innovations: ["Redesigned RDNA compute unit (dual-CU work group)", "New multi-level cache hierarchy", "GDDR6 memory", "PCIe 4.0", "Large perf-per-watt gain over GCN"]
precision_support: ["FP32", "FP16"]
memory_tech: "GDDR6"
interconnect: "PCIe 4.0"
tags: [amd, rdna, navi, gaming]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/RDNA_(microarchitecture)", title: "RDNA (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://www.amd.com/system/files/documents/rdna-whitepaper.pdf", title: "AMD RDNA Architecture Whitepaper", trust: 0.95 }
---

## What Changed
RDNA (Radeon DNA) was a clean break from GCN for the **gaming** market. AMD rebuilt the compute unit
to issue work more efficiently, reworked the cache hierarchy to lower latency, and targeted much better
**performance-per-clock and per-watt** rather than GCN's wide-but-inefficient compute arrays. On TSMC
7nm with **GDDR6** and **PCIe 4.0**, the RX 5700 XT closed much of the gap with NVIDIA's mainstream
cards. RDNA 1 had **no dedicated ray-tracing or matrix hardware** — it was a pure raster-gaming
architecture — but it established the compute-unit and cache design that RDNA 2 and 3 would extend, and
it let AMD run a separate, compute-only line (CDNA) for the datacenter instead of compromising one
architecture for both.
