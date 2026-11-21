---
id: gpu-architecture/pascal
type: gpu-architecture
slug: pascal
schema_version: 1.0
title: "NVIDIA Pascal"
name: "Pascal"
vendor: NVIDIA
codename: "GP100"
year: 2016
predecessor: gpu-architecture/maxwell
successor: gpu-architecture/volta
process_node: "TSMC 16nm FinFET"
segment: "consumer + datacenter"
representative_gpus: []
key_innovation: "The move to 16 nm FinFET, plus NVLink and HBM2 on Tesla P100, built the GPU for multi-GPU datacenter servers."
innovations: ["NVLink GPU-to-GPU interconnect (first introduced with Tesla P100)", "HBM2 stacked memory on Tesla P100", "FP16 arithmetic at up to twice the FP32 rate (GP100)", "Unified Memory with page faulting and migration", "GDDR5X on GeForce GTX 1080"]
precision_support: ["FP64", "FP32", "FP16"]
memory_tech: "HBM2 (Tesla P100) / GDDR5X (GeForce GTX 1080)"
interconnect: "NVLink (Tesla P100) / PCIe Gen 3"
tags: [nvidia, pascal, nvlink, hbm2, fp16]
updated: '2026-11-21'
sources:
  - { url: "https://images.nvidia.com/content/pdf/tesla/whitepaper/pascal-architecture-whitepaper.pdf", title: "NVIDIA Tesla P100 Pascal Architecture Whitepaper", trust: 0.95 }
  - { url: "https://nvidianews.nvidia.com/news/a-quantum-leap-in-gaming:-nvidia-introduces-geforce-gtx-1080", title: "A Quantum Leap in Gaming: NVIDIA Introduces GeForce GTX 1080 (May 6, 2016)", trust: 0.95 }
  - { url: "https://images.nvidia.com/content/volta-architecture/pdf/volta-architecture-whitepaper.pdf", title: "NVIDIA Tesla V100 Volta Architecture Whitepaper", trust: 0.95 }
---

## What Changed
Pascal moved to TSMC's **16 nm FinFET** process after two generations on 28 nm. The **Tesla P100**
(GP100) aimed it at multi-GPU servers.

- **NVLink**, first introduced in 2016 with Tesla P100, gives GPU-to-GPU bandwidth well above PCIe
  Gen 3; NVIDIA's DGX-1 links eight P100s with it.
- **HBM2**: NVIDIA states P100 was the first GPU accelerator to use HBM2 (16 GB in four stacks).
- **FP16**: GP100 runs two FP16 operations per instruction, up to twice the FP32 rate.
- **Unified Memory** gained page faulting, so data migrates between CPU and GPU on demand.

On the consumer side, NVIDIA announced the **GeForce GTX 1080** on May 6, 2016 as the first
Pascal gaming GPU, with 8 GB of GDDR5X memory.
