---
id: gpu-architecture/kepler
type: gpu-architecture
slug: kepler
schema_version: 3.0
title: NVIDIA Kepler
name: Kepler
vendor: NVIDIA
codename: GK104 / GK110 / GK210
year: 2012
process_node: TSMC 28nm
segment: consumer + datacenter
representative_gpus: []
key_innovation: The SMX streaming multiprocessor ran more cores at the lower GPU clock instead of a doubled shader clock; NVIDIA states its priority for Kepler was performance per watt.
innovations:
- SMX streaming multiprocessor
- GPU Boost dynamic clocking
- Dynamic Parallelism (GPU launches its own work)
- Hyper-Q (32 hardware work queues)
precision_support:
- FP64
- FP32
memory_tech: GDDR5
interconnect: PCI Express Gen 3
tags:
- nvidia
- kepler
- cuda
- datacenter
updated: '2026-11-21'
sources:
- url: https://nvidianews.nvidia.com/news/nvidia-launches-first-geforce-gpus-based-on-next-generation-kepler-architecture
  title: NVIDIA Launches First GeForce GPUs Based on Next-Generation Kepler Architecture (March 22, 2012)
  trust: 0.95
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/documents/NVIDIA-Kepler-GK110-GK210-Architecture-Whitepaper.pdf
  title: NVIDIA Kepler GK110/GK210 Architecture Whitepaper
  trust: 0.95
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/tesla-product-literature/TeslaK80-datasheet.pdf
  title: NVIDIA Tesla K40 and K80 GPU Accelerators Datasheet
  trust: 0.95
- url: https://images.nvidia.com/aem-dam/en-zz/Solutions/data-center/nvidia-ampere-architecture-whitepaper.pdf
  title: NVIDIA A100 Tensor Core GPU Architecture Whitepaper
  trust: 0.95
---

## What Changed

NVIDIA launched Kepler on March 22, 2012 with the **GeForce GTX 680**, built on TSMC's 28 nm process.
NVIDIA states that its priority for Kepler was **performance per watt**.

- **SMX** runs its cores at the primary GPU clock rather than the doubled shader clock of earlier
  GPUs, using more cores at a lower, less power-hungry clock.
- **GPU Boost** raises the core clock while power and thermal headroom remain.
- **Dynamic Parallelism** (GK110 and GK210) lets a running kernel launch further kernels without
  the CPU.
- **Hyper-Q** gives the host 32 hardware-managed work queues to the GPU, where Fermi had one.

The datacenter **Tesla K40** (GK110B) and dual-GPU **Tesla K80** (two GK210) carry GDDR5 memory.
Kepler predates Tensor Cores, which NVIDIA first introduced with the Volta architecture.
