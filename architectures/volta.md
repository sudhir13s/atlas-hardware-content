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
representative_gpus: ["Tesla V100 (2017)", "Titan V (2017)", "Tesla V100S (2019)"]
key_innovation: "First-generation Tensor Cores — dedicated matrix-multiply-accumulate units that made mixed-precision deep learning dramatically faster."
innovations: ["1st-generation Tensor Cores (mixed-precision matrix math)", "Independent thread scheduling per thread", "NVLink 2.0", "HBM2 with higher bandwidth"]
precision_support: ["FP64", "FP32", "FP16", "Tensor-FP16"]
memory_tech: "HBM2"
interconnect: "NVLink 2.0"
tags: [nvidia, volta, tensor-cores, v100, hbm2]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Volta_(microarchitecture)", title: "Volta (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://images.nvidia.com/content/volta-architecture/pdf/volta-architecture-whitepaper.pdf", title: "NVIDIA Tesla V100 Volta Architecture Whitepaper", trust: 0.95 }
---

## What Changed
Volta is the architecture that made NVIDIA the default AI-training platform. Its defining feature was
the **first-generation Tensor Core**: a hardware unit that computes a small matrix multiply-accumulate
(FP16 inputs, FP32 accumulation) in one operation, delivering an order-of-magnitude throughput gain
on the dense linear algebra that dominates neural-network training. Volta also added **independent
thread scheduling**, giving each thread its own program counter and enabling finer-grained
synchronization, and upgraded to **NVLink 2.0** with more links and bandwidth. The Tesla V100 became
the standard cloud training GPU for years and powered the models that kicked off the large-language-model
era. Volta was effectively datacenter-only (the Titan V being the lone prosumer card), signaling that
NVIDIA's compute and gaming lines were beginning to diverge.
