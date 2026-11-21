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
representative_gpus: ["nvidia-h100-sxm", "nvidia-h100-pcie", "nvidia-h200"]
key_innovation: "FP8 Tensor Cores paired with the Transformer Engine, which chooses between FP8 and 16-bit calculations layer by layer for transformer training and inference."
innovations: ["Fourth-generation Tensor Cores", "FP8 (E4M3 and E5M2) precision", "Transformer Engine (dynamic FP8/16-bit management)", "Fourth-generation NVLink and the NVLink Switch System", "HBM3 memory (H100 SXM5)", "DPX instructions for dynamic programming", "Confidential Computing"]
precision_support: ["FP64", "TF32", "BF16", "FP16", "FP8", "INT8"]
memory_tech: "HBM3 (H100 SXM5) / HBM2e (H100 PCIe) / HBM3e (H200)"
interconnect: "Fourth-generation NVLink, third-generation NVSwitch, PCIe Gen 5"
tags: [nvidia, hopper, h100, fp8, transformer-engine, hbm3]
updated: '2026-11-21'
sources:
  - { url: "https://resources.nvidia.com/en-us-hopper-architecture/nvidia-h100-tensor-c", title: "NVIDIA H100 Tensor Core GPU Architecture Whitepaper", trust: 0.95 }
  - { url: "https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/", title: "NVIDIA Hopper Architecture In-Depth (NVIDIA Technical Blog, March 22, 2022)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/technologies/hopper-architecture/", title: "NVIDIA Hopper Architecture", trust: 0.95 }
  - { url: "https://nvidianews.nvidia.com/news/nvidia-supercharges-hopper-the-worlds-leading-ai-computing-platform", title: "NVIDIA Supercharges Hopper (H200 announcement, November 13, 2023)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/h200/", title: "NVIDIA H200 Tensor Core GPU", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/grace-hopper-superchip/", title: "NVIDIA GH200 Grace Hopper Superchip", trust: 0.95 }
---

## What Changed
Hopper's H100 (GH100, TSMC 4N) adds **FP8** to its **fourth-generation Tensor Cores** in two
formats: **E4M3** (more precision) and **E5M2** (more range).

- **Transformer Engine** chooses between FP8 and 16-bit calculations per layer and handles the
  re-casting and scaling. NVIDIA states FP8 halves storage and doubles throughput compared with
  FP16 or BF16.
- **Fourth-generation NVLink** gives 900 GB/s per GPU; the **NVLink Switch System** connects up to
  256 GPUs across nodes.
- **DPX instructions** speed up dynamic-programming algorithms such as Smith-Waterman.
- **Confidential Computing** runs workloads in GPU trusted execution environments.

H100 SXM5 uses 80 GB of HBM3 and H100 PCIe 80 GB of HBM2e. The **H200**, announced on November
13, 2023, keeps Hopper with 141 GB of HBM3e at 4.8 TB/s. The **GH200 Grace Hopper Superchip**
joins a Hopper GPU to an Arm-based Grace CPU over 900 GB/s NVLink-C2C.
