---
id: gpu-architecture/hopper
type: gpu-architecture
slug: hopper
schema_version: 1.0
title: "NVIDIA Hopper"
name: "Hopper"
vendor: NVIDIA
codename: "GH100"
year: 2022
predecessor: gpu-architecture/ampere
successor: gpu-architecture/blackwell
process_node: "TSMC 4N"
segment: "datacenter"
representative_gpus: ["H100 SXM (2022)", "H100 PCIe (2022)", "H200 (2023)", "GH200 Grace Hopper Superchip (2023)"]
key_innovation: "FP8 precision paired with the Transformer Engine, which dynamically manages FP8/FP16 to speed up transformer training and inference."
innovations: ["4th-generation Tensor Cores", "FP8 (E4M3 / E5M2) precision", "Transformer Engine (dynamic FP8/FP16 management)", "NVLink 4.0 + external NVLink Switch", "HBM3 memory", "DPX instructions for dynamic programming", "Confidential Computing"]
precision_support: ["FP64", "TF32", "BF16", "FP16", "FP8", "INT8"]
memory_tech: "HBM3 (H100) / HBM3e (H200)"
interconnect: "NVLink 4.0, NVSwitch, PCIe 5.0"
tags: [nvidia, hopper, h100, fp8, transformer-engine, hbm3]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Hopper_(microarchitecture)", title: "Hopper (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://resources.nvidia.com/en-us-tensor-core/gtc22-whitepaper-hopper", title: "NVIDIA H100 Tensor Core GPU Architecture Whitepaper", trust: 0.95 }
---

## What Changed
Hopper is the architecture behind the H100, the GPU most identified with the generative-AI boom. Its
signature feature is the **Transformer Engine**, which combines **FP8** precision (two variants, E4M3
and E5M2) with per-layer statistics that dynamically choose FP8 or FP16 to preserve accuracy — roughly
doubling transformer throughput over BF16. Hopper's **fourth-generation Tensor Cores**, **HBM3**
memory, and **NVLink 4.0** with an external **NVLink Switch** let dozens of GPUs act as one large
memory-coherent accelerator, which is how frontier models are trained. It also added **DPX
instructions** for dynamic-programming algorithms and hardware **confidential computing**. The 2023
**H200** refresh kept the Hopper architecture but upgraded to faster, larger **HBM3e**, and **GH200**
fused a Hopper GPU with an Arm-based Grace CPU over NVLink.
