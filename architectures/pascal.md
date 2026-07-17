---
id: gpu-architecture/pascal
type: gpu-architecture
slug: pascal
schema_version: 1.0
title: "NVIDIA Pascal"
name: "Pascal"
vendor: NVIDIA
codename: "GP1xx"
year: 2016
predecessor: gpu-architecture/maxwell
successor: gpu-architecture/volta
process_node: "TSMC 16nm FinFET"
segment: "consumer + datacenter"
representative_gpus: ["GeForce GTX 1080 (2016)", "GeForce GTX 1080 Ti (2017)", "Tesla P100 (2016)", "Tesla P40 (2016)"]
key_innovation: "The FinFET shrink plus NVLink 1.0 and HBM2 (on P100) turned the GPU into a scalable datacenter compute node."
innovations: ["NVLink 1.0 high-bandwidth GPU-to-GPU interconnect", "HBM2 stacked memory on Tesla P100", "Native FP16 throughput for deep learning", "Unified Memory with page migration", "GDDR5X on GeForce"]
precision_support: ["FP64", "FP32", "FP16"]
memory_tech: "HBM2 (P100) / GDDR5X (GeForce)"
interconnect: "NVLink 1.0 (P100) / PCIe 3.0"
tags: [nvidia, pascal, nvlink, hbm2, fp16]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Pascal_(microarchitecture)", title: "Pascal (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://images.nvidia.com/content/pdf/tesla/whitepaper/pascal-architecture-whitepaper.pdf", title: "NVIDIA Tesla P100 Pascal Architecture Whitepaper", trust: 0.95 }
---

## What Changed
Pascal moved to the **16nm FinFET** process, a genuine node shrink after two generations on 28nm,
and used the transistor budget to attack datacenter scale-out. The Tesla P100 introduced **NVLink
1.0**, a high-bandwidth coherent interconnect that let GPUs talk to each other far faster than PCIe
allowed, and **HBM2** stacked memory for a large jump in bandwidth. Pascal also added first-class
**FP16 throughput**, the beginning of NVIDIA treating reduced precision as a deep-learning feature
rather than an afterthought. Consumer Pascal (GTX 1080, 1080 Ti) was a landmark gaming generation,
but P100 was the strategic piece: it made the GPU a building block you could wire into an 8-GPU
server, which is exactly how large-model training would soon be done.
