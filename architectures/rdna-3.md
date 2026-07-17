---
id: gpu-architecture/rdna-3
type: gpu-architecture
slug: rdna-3
schema_version: 1.0
title: "AMD RDNA 3"
name: "RDNA 3"
vendor: AMD
codename: "Navi 3x"
year: 2022
predecessor: gpu-architecture/rdna-2
process_node: "TSMC 5nm (GCD) + 6nm (MCD)"
segment: "consumer"
representative_gpus: ["Radeon RX 7900 XTX (2022)", "Radeon RX 7900 XT (2022)", "Radeon RX 7800 XT (2023)"]
key_innovation: "The first chiplet-based consumer GPU: a 5nm graphics compute die surrounded by 6nm memory-cache dies, plus dedicated AI accelerators."
innovations: ["Chiplet design (GCD + memory-cache dies)", "Dedicated AI accelerators (WMMA / Wave Matrix Multiply-Accumulate)", "2nd-generation Ray Accelerators", "DisplayPort 2.1", "Decoupled shader and front-end clocks"]
precision_support: ["FP32", "FP16", "BF16", "INT8", "INT4"]
memory_tech: "GDDR6"
interconnect: "PCIe 4.0"
tags: [amd, rdna-3, navi, chiplet, wmma]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/RDNA_3", title: "RDNA 3 — Wikipedia", trust: 0.8 }
  - { url: "https://www.amd.com/en/technologies/rdna-3", title: "AMD RDNA 3 Architecture", trust: 0.9 }
---

## What Changed
RDNA 3 brought **chiplets** — long used in AMD's Ryzen and EPYC CPUs — to a consumer GPU for the first
time. The Radeon RX 7900 series is one **5nm Graphics Compute Die (GCD)** surrounded by several **6nm
Memory Cache Dies (MCDs)** holding the Infinity Cache and memory controllers, letting AMD build the
memory subsystem on a cheaper node and improve yields. RDNA 3 also added **dedicated AI accelerators**
(WMMA instructions) that speed up matrix math with BF16/INT8, a first for AMD's gaming line, along with
**second-generation Ray Accelerators** and decoupled shader/front-end clocks. It is still a gaming
architecture rather than a training part, but the chiplet approach and on-die AI units point at where
consumer GPUs are heading for local inference.
