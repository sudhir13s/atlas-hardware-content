---
id: gpu-architecture/volta
type: gpu-architecture
slug: volta
schema_version: 1.0
title: "NVIDIA Volta"
name: "Volta"
vendor: NVIDIA
codename: "GV100"
year: 2017
predecessor: gpu-architecture/pascal
successor: gpu-architecture/turing
process_node: "TSMC 12nm FFN"
segment: "datacenter"
representative_gpus: ["nvidia-v100-16gb", "nvidia-v100-32gb"]
key_innovation: "Tensor Cores: units that perform a 4x4 matrix multiply-accumulate on FP16 inputs with FP16 or FP32 accumulation."
innovations: ["Tensor Cores (mixed-precision FP16/FP32 matrix math)", "Independent thread scheduling", "Second-generation NVLink", "Faster HBM2 (900 GB/s on Tesla V100)"]
precision_support: ["FP64", "FP32", "FP16", "FP16 Tensor Core with FP32 accumulation"]
memory_tech: "HBM2"
interconnect: "Second-generation NVLink / PCIe Gen3"
tags: [nvidia, volta, tensor-cores, v100, hbm2]
updated: '2026-11-21'
sources:
  - { url: "https://images.nvidia.com/content/volta-architecture/pdf/volta-architecture-whitepaper.pdf", title: "NVIDIA Tesla V100 Volta Architecture Whitepaper", trust: 0.95 }
  - { url: "https://images.nvidia.com/content/technologies/volta/pdf/volta-v100-datasheet-update-us-1165301-r5.pdf", title: "NVIDIA V100 Tensor Core GPU Datasheet", trust: 0.95 }
---

## What Changed
Volta's **Tensor Core** performs a 4x4 matrix multiply-accumulate in hardware, taking FP16 inputs
and accumulating in FP16 or FP32. Tesla V100 has 640 of them.

- **Throughput**: NVIDIA states up to 12x higher peak TFLOPS for training and 6x for inference
  compared with Pascal.
- **Independent thread scheduling** keeps a program counter and call stack per thread; NVIDIA
  states GV100 is the first GPU to support it.
- **Second-generation NVLink** and faster **HBM2** (900 GB/s peak on Tesla V100).

V100 ships with 16 GB or 32 GB of HBM2, in SXM2 (NVLink) and PCIe Gen3 boards. The later
**V100S PCIe** has 32 GB at 1134 GB/s.
