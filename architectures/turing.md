---
id: gpu-architecture/turing
type: gpu-architecture
slug: turing
schema_version: 1.0
title: "NVIDIA Turing"
name: "Turing"
vendor: NVIDIA
codename: "TU1xx"
year: 2018
predecessor: gpu-architecture/volta
successor: gpu-architecture/ampere
process_node: "TSMC 12nm FFN"
segment: "consumer + datacenter"
representative_gpus: ["GeForce RTX 2080 Ti (2018)", "GeForce RTX 2080 (2018)", "Tesla T4 (2018)", "Quadro RTX 8000 (2018)"]
key_innovation: "First RT Cores for hardware-accelerated ray tracing, alongside second-generation Tensor Cores with INT8/INT4 inference paths."
innovations: ["1st-generation RT Cores (hardware ray tracing)", "2nd-generation Tensor Cores", "INT8 and INT4 integer inference", "GDDR6 memory", "DLSS (AI upscaling debut)"]
precision_support: ["FP32", "FP16", "INT8", "INT4"]
memory_tech: "GDDR6"
interconnect: "NVLink 2.0 (high-end) / PCIe 3.0"
tags: [nvidia, turing, rt-cores, tensor-cores, int8]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Turing_(microarchitecture)", title: "Turing (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://images.nvidia.com/aem-dam/en-zz/Solutions/design-visualization/technologies/turing-architecture/NVIDIA-Turing-Architecture-Whitepaper.pdf", title: "NVIDIA Turing Architecture Whitepaper", trust: 0.95 }
---

## What Changed
Turing brought the Tensor Core down from the datacenter into consumer GeForce cards and added a second
dedicated unit type: the **RT Core** for hardware ray tracing. Its **second-generation Tensor Cores**
extended to **INT8 and INT4** integer paths, making Turing a strong inference architecture — the Tesla
T4, a low-power single-slot card, became a ubiquitous inference workhorse in datacenters. Turing also
debuted **DLSS**, using the Tensor Cores to upscale rendered frames with a neural network, the first
mainstream example of AI hardware improving graphics. With three specialized execution paths (CUDA
cores, Tensor Cores, RT Cores) on one die, Turing established the multi-engine GPU template that every
later NVIDIA consumer architecture would follow.
