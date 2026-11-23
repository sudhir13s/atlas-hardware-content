---
id: gpu-architecture/turing
type: gpu-architecture
slug: turing
schema_version: 3.0
title: NVIDIA Turing
name: Turing
vendor: NVIDIA
codename: TU102 / TU104 / TU106
year: 2018
predecessors:
- gpu-architecture/volta
process_node: TSMC 12nm FFN
segment: consumer + datacenter
representative_gpus:
- gpu/nvidia-t4
key_innovation: RT Cores for hardware-accelerated ray tracing, alongside second-generation Tensor Cores that add INT8 and INT4 modes for inference.
innovations:
- First-generation RT Cores (hardware ray tracing)
- Second-generation Tensor Cores
- INT8 and INT4 Tensor Core modes
- GDDR6 memory
- Deep Learning Super Sampling (DLSS)
precision_support:
- FP32
- FP16
- INT8
- INT4
memory_tech: GDDR6
interconnect: Second-generation NVLink (TU102, TU104) / PCI Express Gen3
tags:
- nvidia
- turing
- rt-cores
- tensor-cores
- int8
updated: '2026-11-21'
sources:
- url: https://images.nvidia.com/aem-dam/en-zz/Solutions/design-visualization/technologies/turing-architecture/NVIDIA-Turing-Architecture-Whitepaper.pdf
  title: NVIDIA Turing Architecture Whitepaper
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/tesla-t4/
  title: NVIDIA T4 Tensor Core GPU
  trust: 0.95
- url: https://www.nvidia.com/content/PDF/nvidia-ampere-ga-102-gpu-architecture-whitepaper-v2.pdf
  title: NVIDIA Ampere GA102 GPU Architecture Whitepaper (Turing generation numbering)
  trust: 0.95
---

## What Changed

Turing put Tensor Cores into **GeForce and Quadro** cards and added a second dedicated unit, the
**RT Core**, which accelerates ray-tracing traversal and ray/triangle tests.

- **Tensor Cores** gain **INT8 and INT4** modes for inference that does not need FP16.
- **DLSS** (Deep Learning Super Sampling) uses the Tensor Cores to build a high-quality frame from
  a lower sample count.
- **GDDR6**: NVIDIA states Turing is the first GPU architecture to support it.
- **Second-generation NVLink** on TU102 and TU104 links two GPUs.

The datacenter **Tesla T4** (TU104) is a 70 W PCIe card with 16 GB of GDDR6 and a PCI Express
Gen3 x16 link, rated at up to 130 TOPS INT8 and 260 TOPS INT4.
