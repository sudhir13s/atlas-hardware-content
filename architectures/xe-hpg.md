---
id: gpu-architecture/xe-hpg
type: gpu-architecture
slug: xe-hpg
schema_version: 1.0
title: "Intel Xe-HPG (Arc Alchemist)"
name: "Xe-HPG (Arc Alchemist)"
vendor: Intel
codename: "Alchemist (DG2)"
year: 2022
predecessor: gpu-architecture/xe
process_node: "TSMC 6nm"
segment: "consumer"
representative_gpus: ["Arc A770 (2022)", "Arc A750 (2022)", "Arc A380 (2022)"]
key_innovation: "Intel's first competitive discrete gaming GPU, adding XMX matrix engines for AI and dedicated hardware ray tracing."
innovations: ["XMX (Xe Matrix Extensions) AI matrix engines", "Hardware ray-tracing units", "XeSS AI-based upscaling", "Full AV1 hardware encode/decode", "Dedicated Xe-cores"]
precision_support: ["FP16", "BF16", "INT8", "INT4"]
memory_tech: "GDDR6"
interconnect: "PCIe 4.0"
tags: [intel, arc, xe-hpg, alchemist, xmx, xess]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Intel_Arc", title: "Intel Arc — Wikipedia", trust: 0.8 }
  - { url: "https://www.intel.com/content/www/us/en/products/docs/discrete-gpus/arc/technology/xe-hpg-microarchitecture.html", title: "Intel Xe-HPG Microarchitecture", trust: 0.85 }
---

## What Changed
Xe-HPG, sold as the **Arc Alchemist** (A-series) GPUs, was Intel's first genuinely competitive
discrete gaming card. Each Xe-core includes **XMX (Xe Matrix Extensions)** engines — matrix-multiply
units analogous to Tensor Cores — which power **XeSS**, Intel's AI upscaler, and give the cards real
low-precision AI throughput (BF16/INT8). Arc also shipped with **hardware ray tracing** and,
notably, **full AV1 hardware encode**, which made the cheap A380 popular for video work before rivals
matched it. Early drivers were rough, especially on older DirectX titles, but Arc established Intel as
a third GPU vendor with a real feature set. For AI, an Arc A770's XMX units and 16 GB of memory make it
a budget option for local inference, though the software ecosystem trails CUDA and ROCm.
