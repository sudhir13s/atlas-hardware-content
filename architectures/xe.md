---
id: gpu-architecture/xe
type: gpu-architecture
slug: xe
schema_version: 1.0
title: "Intel Xe"
name: "Xe"
vendor: Intel
codename: "Xe-LP (Gen12)"
year: 2020
successor: gpu-architecture/xe-hpg
process_node: "Intel 10nm SuperFin"
segment: "consumer"
representative_gpus: ["Iris Xe Graphics (Tiger Lake, 2020)", "Iris Xe MAX / DG1 (2020)", "Server GPU SG1 (2021)"]
key_innovation: "A single, scalable Xe GPU architecture intended to span integrated graphics, discrete gaming, and datacenter compute under one microarchitecture and the oneAPI software stack."
innovations: ["Unified, scalable Xe architecture (LP / HPG / HPC tiers)", "Intel's return to discrete GPUs (DG1)", "oneAPI cross-architecture programming model", "Foundation for later XMX matrix engines"]
precision_support: ["FP32", "FP16", "INT8"]
memory_tech: "LPDDR4X / GDDR6"
interconnect: "PCIe 4.0"
tags: [intel, xe, dg1, oneapi]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Intel_Xe", title: "Intel Xe — Wikipedia", trust: 0.8 }
  - { url: "https://www.intel.com/content/www/us/en/products/docs/discrete-gpus/arc/technology/xe-hpg-microarchitecture.html", title: "Intel Xe Architecture Overview", trust: 0.85 }
---

## What Changed
Xe marked **Intel's re-entry into discrete GPUs** and its bet on a **single scalable architecture**
spanning four tiers: Xe-LP (low power, integrated and entry discrete), Xe-HPG (high-performance
gaming), Xe-HP, and Xe-HPC (datacenter). The first products were the Iris Xe integrated graphics in
Tiger Lake laptops and the modest **DG1** discrete card — not competitive with high-end NVIDIA or AMD,
but proof Intel could ship a standalone GPU again. The strategic pieces were the **oneAPI** software
stack, meant to program CPUs, GPUs, and accelerators with one model, and the groundwork for the **XMX
matrix engines** that later Xe variants (Arc, and the datacenter Ponte Vecchio) would use for AI. Xe
was the platform; Arc and Gaudi are where Intel's AI-relevant hardware actually landed.
