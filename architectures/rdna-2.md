---
id: gpu-architecture/rdna-2
type: gpu-architecture
slug: rdna-2
schema_version: 1.0
title: "AMD RDNA 2"
name: "RDNA 2"
vendor: AMD
codename: "Navi 2x"
year: 2020
predecessor: gpu-architecture/rdna
successor: gpu-architecture/rdna-3
process_node: "TSMC 7nm"
segment: "consumer"
representative_gpus: ["Radeon RX 6900 XT (2020)", "Radeon RX 6800 XT (2020)", "Radeon RX 6700 XT (2021)", "PlayStation 5 / Xbox Series X GPU (2020)"]
key_innovation: "Infinity Cache — a large on-die last-level cache — plus first-generation Ray Accelerators for hardware ray tracing."
innovations: ["Infinity Cache (large on-die LLC)", "Ray Accelerators (hardware ray tracing)", "Higher clock speeds", "Smart Access Memory (Resizable BAR)", "Powers PS5 and Xbox Series consoles"]
precision_support: ["FP32", "FP16", "INT8", "INT4"]
memory_tech: "GDDR6"
interconnect: "PCIe 4.0"
tags: [amd, rdna-2, navi, ray-tracing, infinity-cache]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/RDNA_2", title: "RDNA 2 — Wikipedia", trust: 0.8 }
  - { url: "https://www.amd.com/en/technologies/rdna-2", title: "AMD RDNA 2 Architecture", trust: 0.9 }
---

## What Changed
RDNA 2 made AMD competitive at the high end again. Its headline feature was **Infinity Cache**, a large
on-die last-level cache that feeds the GPU from fast local SRAM and reduces reliance on external memory
bandwidth — letting AMD hit high performance on a 256-bit GDDR6 bus. It added **Ray Accelerators**,
AMD's first hardware ray-tracing units, one per compute unit, and pushed clocks substantially higher on
the same 7nm node. RDNA 2 also went into the **PlayStation 5 and Xbox Series X/S**, giving the
architecture enormous reach. For AI it added **INT8/INT4** integer paths useful for inference, though
AMD's serious machine-learning silicon remained the separate CDNA line; RDNA 2 was still a
gaming-first design.
