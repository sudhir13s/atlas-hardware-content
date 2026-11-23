---
id: gpu-architecture/xe-hpg
type: gpu-architecture
slug: xe-hpg
schema_version: 3.0
title: Intel Xe-HPG (Arc Alchemist)
name: Xe-HPG (Arc Alchemist)
vendor: Intel
codename: Alchemist (DG2)
year: 2022
predecessors:
- gpu-architecture/xe
process_node: TSMC N6
segment: consumer
representative_gpus:
- gpu/intel-arc-a770
key_innovation: Xe-cores that pair 16 vector engines with 16 XMX matrix engines and a ray-tracing unit, for Intel Arc A-series discrete GPUs.
innovations:
- 'Xe-core: 16 Xe Vector Engines (XVE) + 16 Intel Xe Matrix Extensions (XMX) engines'
- Ray tracing unit per Xe-core
- Intel Xe Super Sampling (XeSS) running on the XMX engines
- AV1 hardware encode and decode
- Up to 32 Xe-cores
precision_support:
- FP32
- FP16
- BF16
- INT8
- INT4
memory_tech: GDDR6
interconnect: PCIe 4.0
tags:
- intel
- arc
- xe-hpg
- alchemist
- xmx
- xess
updated: '2026-11-21'
sources:
- url: https://www.intel.com/content/www/us/en/developer/articles/technical/introduction-to-the-xe-hpg-architecture.html
  title: 'Intel: Introduction to the Xe-HPG Architecture'
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/products/sku/227959/intel-arc-a380-graphics/specifications.html
  title: Intel Arc A380 Graphics specifications
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/products/details/discrete-gpus/arc/desktop/a-series.html
  title: Intel Arc A-Series Graphics for Desktops
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/docs/oneapi/optimization-guide-gpu/2025-0/intel-xe-gpu-architecture.html
  title: 'Intel oneAPI GPU Optimization Guide: Intel Xe GPU Architecture'
  trust: 0.95
---

## What Changed

Xe-HPG is the high-performance gaming member of Intel's Xe family. It powers the **Intel Arc
A-series** (formerly code named Alchemist, also called DG2), built on **TSMC N6**; Intel lists the Arc
A380 as launched in Q2 2022.

- **Xe-core:** 16 vector engines, 16 **XMX** matrix engines, a load/store unit and a shared L1 cache,
  with a dedicated ray-tracing unit.
- **AI:** the XMX engines support FP16, BF16, INT8, INT4 and INT2 through the DPAS instruction. They
  also run **XeSS**, Intel's upscaler.
- **Memory and I/O:** **GDDR6**; the Arc A770 comes with 8 GB or 16 GB, and the Arc A380 lists
  PCI Express 4.0.
- **Media:** AV1 hardware encode and decode.
