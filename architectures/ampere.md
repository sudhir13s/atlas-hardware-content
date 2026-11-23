---
id: gpu-architecture/ampere
type: gpu-architecture
slug: ampere
schema_version: 3.0
title: NVIDIA Ampere
name: Ampere
vendor: NVIDIA
codename: GA100 / GA102
year: 2020
predecessors:
- gpu-architecture/turing
process_node: TSMC 7nm N7 (A100) / Samsung 8nm 8N (GA102)
segment: consumer + datacenter
representative_gpus:
- gpu/nvidia-a100-40gb
- gpu/nvidia-a100-80gb
- gpu/nvidia-rtx-3090
- gpu/nvidia-rtx-3080
key_innovation: Third-generation Tensor Cores added TF32, BF16, FP64 and 2:4 fine-grained structured sparsity, and the A100 introduced Multi-Instance GPU (MIG) partitioning.
innovations:
- Third-generation Tensor Cores
- TF32 Tensor Core format (FP32 range, FP16 precision)
- BF16 Tensor Core support
- 2:4 fine-grained structured sparsity
- Multi-Instance GPU (MIG)
- Third-generation NVLink
precision_support:
- FP64
- TF32
- BF16
- FP16
- INT8
- INT4
memory_tech: HBM2 (A100 40GB) / HBM2e (A100 80GB) / GDDR6X (GeForce RTX 3090, 3080)
interconnect: Third-generation NVLink / PCIe Gen 4
tags:
- nvidia
- ampere
- a100
- tf32
- bf16
- sparsity
- mig
updated: '2026-11-21'
sources:
- url: https://images.nvidia.com/aem-dam/en-zz/Solutions/data-center/nvidia-ampere-architecture-whitepaper.pdf
  title: NVIDIA A100 Tensor Core GPU Architecture Whitepaper
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/a100/
  title: NVIDIA A100 Tensor Core GPU
  trust: 0.95
- url: https://www.nvidia.com/content/PDF/nvidia-ampere-ga-102-gpu-architecture-whitepaper-v2.pdf
  title: NVIDIA Ampere GA102 GPU Architecture Whitepaper
  trust: 0.95
---

## What Changed

The **A100** (GA100, TSMC 7 nm N7) brought **third-generation Tensor Cores** with new formats.

- **TF32** has FP32's range with FP16's precision; NVIDIA states A100 uses TF32 Tensor Cores for
  FP32 work by default, with no change to user scripts.
- **BF16** runs at the same Tensor Core rate as FP16, and **FP64** Tensor Core operations serve HPC.
- **2:4 fine-grained structured sparsity** (two non-zero weights in every four) doubles Tensor Core
  throughput on pruned networks.
- **Multi-Instance GPU (MIG)** splits one A100 into as many as seven isolated GPU instances.
- **Third-generation NVLink** and **PCIe Gen 4** connect A100 GPUs.

The A100 ships with 40 GB of HBM2 or 80 GB of HBM2e. The consumer **GA102** (GeForce RTX 3090,
RTX 3080) uses Samsung's 8 nm 8N process and GDDR6X memory.
