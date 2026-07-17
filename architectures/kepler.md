---
id: gpu-architecture/kepler
type: gpu-architecture
slug: kepler
schema_version: 1.0
title: "NVIDIA Kepler"
name: "Kepler"
vendor: NVIDIA
codename: "GK1xx"
year: 2012
successor: gpu-architecture/maxwell
process_node: "TSMC 28nm"
segment: "consumer + datacenter"
representative_gpus: ["GeForce GTX 680 (2012)", "GeForce GTX 780 Ti (2013)", "Tesla K40 (2013)", "Tesla K80 (2014)"]
key_innovation: "The SMX streaming multiprocessor traded per-core clock for many more, lower-clocked cores, prioritizing performance-per-watt."
innovations: ["SMX streaming multiprocessor", "GPU Boost dynamic clocking", "Dynamic Parallelism (GPU launches its own work)", "Hyper-Q multiple hardware work queues"]
precision_support: ["FP64", "FP32"]
memory_tech: "GDDR5"
interconnect: "PCIe 3.0"
tags: [nvidia, kepler, cuda, datacenter]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Kepler_(microarchitecture)", title: "Kepler (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://www.nvidia.com/content/PDF/kepler/NVIDIA-Kepler-GK110-Architecture-Whitepaper.pdf", title: "NVIDIA Kepler GK110 Architecture Whitepaper", trust: 0.95 }
---

## What Changed
Kepler was the first NVIDIA generation designed around **performance-per-watt** rather than raw
per-core clock speed. Its SMX multiprocessor packed far more CUDA cores than Fermi's SM but ran them
at a lower, more efficient clock, and GPU Boost opportunistically raised clocks within the power and
thermal budget. Two features pointed at the future of GPU compute: **Dynamic Parallelism**, letting
a running kernel launch further kernels without a CPU round trip, and **Hyper-Q**, exposing multiple
hardware work queues so more of the chip stayed busy. The Tesla K40 and dual-GPU K80 made Kepler the
workhorse of early deep-learning research — AlexNet-era training ran on Kepler-class cards — but the
architecture had **no tensor/matrix units**; all math went through the general FP32/FP64 datapath.
