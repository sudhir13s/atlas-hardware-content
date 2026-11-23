---
id: gpu-architecture/cdna-2
type: gpu-architecture
slug: cdna-2
schema_version: 3.0
title: AMD CDNA 2
name: CDNA 2
vendor: AMD
year: 2021
predecessors:
- gpu-architecture/cdna
process_node: TSMC 6nm
segment: datacenter
representative_gpus:
- gpu/amd-mi250x
- gpu/amd-mi210
key_innovation: Two Graphics Compute Dies in one package joined by in-package Infinity Fabric, with FP64 matrix instructions and a coherent link to optimized AMD EPYC CPUs.
innovations:
- Two Graphics Compute Dies (GCDs) per package on MI250 and MI250X
- FP64 matrix instructions (twice the throughput of FP64 vector instructions)
- Packed FP32 instructions
- Coherent Infinity Fabric link to optimized 3rd Gen AMD EPYC processors (MI250X)
- 3rd Gen AMD Infinity Architecture
precision_support:
- FP64
- FP32
- FP16
- BF16
- INT8
- INT4
memory_tech: HBM2e
interconnect: Infinity Fabric, PCIe 4.0
tags:
- amd
- cdna-2
- mi250x
- fp64
- exascale
updated: '2026-11-21'
sources:
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-business-docs/white-papers/amd-cdna2-white-paper.pdf
  title: AMD CDNA 2 Architecture white paper
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi200/mi250x.html
  title: AMD Instinct MI250X specifications
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi200/mi210.html
  title: AMD Instinct MI210 specifications
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-tech-docs/white-papers/amd-cdna-3-white-paper.pdf
  title: AMD CDNA 3 Architecture white paper (CDNA 2 background)
  trust: 0.95
---

## What Changed

CDNA 2 powers the **Instinct MI200 Series**. The MI250X launched on 8 November 2021 on TSMC 6nm; the
single-die MI210 PCIe card followed on 22 March 2022.

- **Two dies:** MI250 and MI250X place two **Graphics Compute Dies** in one OAM module, linked
  in-package by Infinity Fabric at up to 400 GB/s; each die appears as a GPU.
- **FP64:** new FP64 matrix instructions give twice the throughput of FP64 vector instructions (95.7
  TFLOPS FP64 matrix on MI250X).
- **Memory:** up to 128 GB of **HBM2e** at 3.2 TB/s per MI250X.
- **Coherency:** the MI250X can share a cache-coherent memory view with optimized 3rd Gen AMD EPYC
  processors. AMD states the MI250X is at the heart of the first exascale system.
