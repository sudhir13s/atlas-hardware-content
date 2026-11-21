---
id: gpu-architecture/ada-lovelace
type: gpu-architecture
slug: ada-lovelace
schema_version: 1.0
title: "NVIDIA Ada Lovelace"
name: "Ada Lovelace"
vendor: NVIDIA
codename: "AD102"
year: 2022
predecessor: gpu-architecture/ampere
successor: gpu-architecture/blackwell
process_node: "TSMC 4N"
segment: "consumer + datacenter"
representative_gpus: ["nvidia-rtx-4090", "nvidia-rtx-4080", "nvidia-l40s"]
key_innovation: "Fourth-generation Tensor Cores with FP8, third-generation RT Cores, and DLSS 3 frame generation, on TSMC 4N."
innovations: ["Third-generation RT Cores", "Fourth-generation Tensor Cores with FP8", "DLSS 3 frame generation (Optical Flow Accelerator)", "Shader Execution Reordering", "Larger L2 cache (96 MB on full AD102)", "AV1 encoding (dual NVENC on RTX 4090 and 4080)"]
precision_support: ["FP32", "FP16", "FP8", "INT8", "INT4"]
memory_tech: "GDDR6X (GeForce RTX 4090, 4080) / GDDR6 with ECC (L40, L40S, L4)"
interconnect: "PCI Express Gen 4"
tags: [nvidia, ada-lovelace, rtx-4090, fp8, dlss3]
updated: '2026-11-21'
sources:
  - { url: "https://images.nvidia.com/aem-dam/Solutions/geforce/ada/nvidia-ada-gpu-architecture.pdf", title: "NVIDIA Ada GPU Architecture Whitepaper", trust: 0.95 }
  - { url: "https://nvidianews.nvidia.com/news/nvidia-delivers-quantum-leap-in-performance-introduces-new-era-of-neural-rendering-with-geforce-rtx-40-series", title: "NVIDIA Introduces GeForce RTX 40 Series (September 20, 2022)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/l40s/", title: "NVIDIA L40S GPU", trust: 0.95 }
---

## What Changed
NVIDIA unveiled Ada Lovelace on September 20, 2022 with the **GeForce RTX 40 Series**, built on a
custom **TSMC 4N** process. NVIDIA states the architecture gives up to a 2x leap in power efficiency.

- **Fourth-generation Tensor Cores** add **FP8**, which halves storage and doubles throughput
  compared with FP16.
- **Third-generation RT Cores** double ray-triangle intersection throughput over Ampere.
- **DLSS 3** uses a new Optical Flow Accelerator to generate whole frames.
- **L2 cache** reaches 96 MB on the full AD102, 16x the 6 MB of GA102.

The datacenter **L40**, **L40S** and **L4** use GDDR6 with ECC. The L40 and L40S are PCIe Gen4
cards, and the L40S specification lists no NVLink support.
