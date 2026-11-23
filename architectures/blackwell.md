---
id: gpu-architecture/blackwell
type: gpu-architecture
slug: blackwell
schema_version: 3.0
title: NVIDIA Blackwell
name: Blackwell
vendor: NVIDIA
year: 2024
predecessors:
- gpu-architecture/hopper
- gpu-architecture/ada-lovelace
process_node: TSMC 4NP
segment: consumer + datacenter
representative_gpus:
- gpu/nvidia-b200
- gpu/nvidia-gb200
- gpu/nvidia-rtx-5090
key_innovation: Two reticle-limited dies joined by a 10 TB/s chip-to-chip link into one GPU, with a second-generation Transformer Engine that adds FP4 and microscaling formats.
innovations:
- FP4 and FP6 Tensor Core formats
- Second-generation Transformer Engine
- Two reticle-limited dies as one GPU (10 TB/s chip-to-chip link)
- Fifth-generation NVLink
- Dedicated decompression engine
- RAS (reliability, availability and serviceability) engine
precision_support:
- FP64
- BF16
- FP16
- FP8
- FP6
- FP4
memory_tech: HBM3E (datacenter) / GDDR7 (GeForce RTX 5090)
interconnect: Fifth-generation NVLink, NVLink Switch; PCI Express Gen 5 (GeForce RTX 5090)
tags:
- nvidia
- blackwell
- b200
- gb200
- fp4
- hbm3e
updated: '2026-11-21'
sources:
- url: https://nvidianews.nvidia.com/news/nvidia-blackwell-platform-arrives-to-power-a-new-era-of-computing
  title: NVIDIA Blackwell Platform Arrives to Power a New Era of Computing (March 18, 2024)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/
  title: NVIDIA Blackwell Architecture
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/gb200-nvl72/
  title: NVIDIA GB200 NVL72
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/hgx/
  title: NVIDIA HGX Platform (HGX B200 specifications)
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5090/
  title: NVIDIA GeForce RTX 5090
  trust: 0.95
---

## What Changed

NVIDIA announced Blackwell on March 18, 2024. A datacenter Blackwell GPU is **two reticle-limited
dies** joined by a **10 TB/s chip-to-chip link** into one unified GPU, with 208 billion transistors
on a custom TSMC 4NP process.

- **Second-generation Transformer Engine** adds **FP4** and community-defined **microscaling**
  formats; the GB200 NVL72 specification also lists FP6 Tensor Core throughput.
- **Fifth-generation NVLink** gives 1.8 TB/s bidirectional per GPU and spans up to 576 GPUs.
- A dedicated **decompression engine** accelerates database queries, and a **RAS engine** flags
  potential faults early.

The **GB200 Grace Blackwell Superchip** pairs two B200 GPUs with one Grace CPU; 36 of them form the
GB200 NVL72 rack. The **GeForce RTX 5090** brings Blackwell to consumers with 32 GB of GDDR7.
