---
id: gpu-architecture/blackwell
type: gpu-architecture
slug: blackwell
schema_version: 1.0
title: "NVIDIA Blackwell"
name: "Blackwell"
vendor: NVIDIA
codename: "GB1xx / B2xx"
year: 2024
predecessor: gpu-architecture/hopper
process_node: "TSMC 4NP"
segment: "consumer + datacenter"
representative_gpus: ["B200 (2024)", "GB200 Grace Blackwell Superchip (2024)", "GeForce RTX 5090 (2025)"]
key_innovation: "A dual-die GPU joined by a ~10 TB/s die-to-die link, with a second-generation Transformer Engine adding FP4 and FP6 microscaling precision."
innovations: ["5th-generation Tensor Cores", "FP4 and FP6 microscaling formats", "2nd-generation Transformer Engine", "Dual-die design (two reticle-limited dies as one GPU via NV-HBI)", "NVLink 5.0", "Dedicated decompression engine", "RAS reliability engine"]
precision_support: ["FP64", "BF16", "FP16", "FP8", "FP6", "FP4"]
memory_tech: "HBM3e"
interconnect: "NVLink 5.0, NVSwitch, PCIe 6.0"
tags: [nvidia, blackwell, b200, gb200, fp4, hbm3e]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)", title: "Blackwell (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://resources.nvidia.com/en-us-blackwell-architecture", title: "NVIDIA Blackwell Architecture Technical Brief", trust: 0.95 }
---

## What Changed
Blackwell broke the single-die ceiling. A datacenter Blackwell GPU is **two reticle-limited dies**
fused by a ~10 TB/s die-to-die interconnect (NV-HBI) and presented to software as **one** GPU with a
unified memory space — the practical answer to how you keep growing when a single die can no longer get
bigger. Its **second-generation Transformer Engine** and **fifth-generation Tensor Cores** add **FP4
and FP6** microscaling formats, cutting the bits per value further for inference and low-precision
training while using block-wise scaling to hold accuracy. **NVLink 5.0** roughly doubles per-GPU
interconnect bandwidth again, and the **GB200** superchip pairs two Blackwell GPUs with a Grace CPU for
rack-scale NVLink domains (GB200 NVL72). A dedicated **decompression engine** and a **RAS engine** for
reliability round it out. The consumer **RTX 5090** (2025) brings the architecture to GeForce.
