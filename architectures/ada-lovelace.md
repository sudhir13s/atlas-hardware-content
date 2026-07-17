---
id: gpu-architecture/ada-lovelace
type: gpu-architecture
slug: ada-lovelace
schema_version: 1.0
title: "NVIDIA Ada Lovelace"
name: "Ada Lovelace"
vendor: NVIDIA
codename: "AD1xx"
year: 2022
predecessor: gpu-architecture/ampere
successor: gpu-architecture/blackwell
process_node: "TSMC 4N"
segment: "consumer + professional"
representative_gpus: ["GeForce RTX 4090 (2022)", "GeForce RTX 4080 (2022)", "RTX 6000 Ada (2022)", "L40S (2023)"]
key_innovation: "An efficiency-focused consumer architecture adding FP8, third-generation RT Cores, and DLSS 3 AI frame generation."
innovations: ["3rd-generation RT Cores", "4th-generation Tensor Cores with FP8", "DLSS 3 AI frame generation", "Shader Execution Reordering", "Large on-die L2 cache", "AV1 dual encoders"]
precision_support: ["FP32", "FP16", "FP8", "INT8", "INT4"]
memory_tech: "GDDR6X"
interconnect: "PCIe 4.0"
tags: [nvidia, ada-lovelace, rtx-4090, fp8, dlss3]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Ada_Lovelace_(microarchitecture)", title: "Ada Lovelace (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://images.nvidia.com/aem-dam/Solutions/geforce/ada/nvidia-ada-gpu-architecture.pdf", title: "NVIDIA Ada GPU Architecture Whitepaper", trust: 0.95 }
---

## What Changed
Ada Lovelace is the consumer and professional-visualization counterpart to Hopper: same **TSMC 4N**
process, but built for graphics and local AI rather than datacenter scale-out. The move from Samsung
8nm (Ampere GeForce) to 4N delivered a large efficiency and clock-speed jump, and a much larger on-die
**L2 cache** cut memory-bandwidth pressure. Its **fourth-generation Tensor Cores** brought **FP8** to
consumer cards, and **third-generation RT Cores** plus **DLSS 3** — which generates entire interpolated
frames with a neural network — pushed real-time ray tracing further. Because Ada lacks NVLink and uses
GDDR6X rather than HBM, it is not a scale-out training part, but a single RTX 4090 or L40S became a
popular choice for local fine-tuning and inference where one card's memory suffices.
