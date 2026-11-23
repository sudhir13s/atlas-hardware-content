---
id: gpu-architecture/xe
type: gpu-architecture
slug: xe
schema_version: 3.0
title: Intel Xe
name: Xe
vendor: Intel
codename: Xe-LP
year: 2020
process_node: Intel 10nm SuperFin
segment: consumer
representative_gpus: []
key_innovation: One Xe GPU architecture with microarchitectures for integrated, discrete gaming and datacenter graphics; its first microarchitecture, Xe-LP, also gave Intel its first Xe-based discrete GPU.
innovations:
- Xe-LP microarchitecture shared by Intel Iris Xe (integrated) and Intel Iris Xe MAX (discrete)
- 'Intel Iris Xe MAX: Intel''s first Xe-based discrete GPU'
- INT8 inference through the DP4a instruction
- oneAPI cross-architecture toolkits
precision_support:
- FP32
- FP16
- INT8
memory_tech: Shared system memory (integrated Iris Xe); dedicated memory (discrete Iris Xe MAX)
interconnect: PCIe 4.0 (Iris Xe MAX)
tags:
- intel
- xe
- dg1
- oneapi
updated: '2026-11-21'
sources:
- url: https://www.intel.com/content/www/us/en/newsroom/news/iris-xe-max-discrete-graphics-deep-link.html
  title: 'Intel Newsroom: Innovation Extends with Intel Iris Xe MAX Graphics and Deep Link (31 October 2020)'
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/docs/oneapi/optimization-guide-gpu/2025-0/intel-xe-gpu-architecture.html
  title: 'Intel oneAPI GPU Optimization Guide: Intel Xe GPU Architecture'
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/developer/articles/technical/introduction-to-the-xe-hpg-architecture.html
  title: 'Intel: Introduction to the Xe-HPG Architecture (Xe-LP comparison table)'
  trust: 0.95
---

## What Changed

Xe is Intel's GPU architecture family, with the Xe-LP, Xe-HPG and Xe-HPC microarchitectures. Intel
describes Xe as spanning integrated, entry discrete, high-end gaming and datacenter graphics.

- **Xe-LP products:** Intel Iris Xe graphics in 11th Gen Intel Core mobile processors, and **Intel Iris
  Xe MAX**, launched 31 October 2020 on Intel 10nm SuperFin with PCIe Gen 4.
- **Discrete:** Intel calls Iris Xe MAX its first Xe-based discrete GPU, part of its strategy to enter
  the discrete graphics market.
- **AI:** Xe-LP runs INT8 inference through the DP4a instruction; the XMX matrix engines came later with
  Xe-HPG.
- **Datacenter:** the Xe-HPC microarchitecture powers the Intel Data Center GPU Max (formerly code
  named Ponte Vecchio).
