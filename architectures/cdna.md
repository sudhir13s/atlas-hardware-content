---
id: gpu-architecture/cdna
type: gpu-architecture
slug: cdna
schema_version: 1.0
title: "AMD CDNA"
name: "CDNA"
vendor: AMD
year: 2020
predecessor: gpu-architecture/gcn
successor: gpu-architecture/cdna-2
process_node: "TSMC 7nm"
segment: "datacenter"
representative_gpus: ["amd-mi100"]
key_innovation: "AMD's compute-only datacenter architecture, adding Matrix Core Engines (MFMA instructions) to GCN-derived compute units and removing the fixed-function graphics hardware."
innovations: ["Matrix Core Engines executing Matrix Fused Multiply-Add (MFMA) instructions", "Fixed-function graphics hardware and display engine removed", "Three Infinity Fabric links per GPU for fully connected four-GPU hives", "PCIe 4.0 host interface"]
precision_support: ["FP64", "FP32", "FP16", "BF16", "INT8", "INT4"]
memory_tech: "HBM2"
interconnect: "Infinity Fabric, PCIe 4.0"
tags: [amd, cdna, mi100, matrix-cores, datacenter]
updated: '2026-11-21'
sources:
  - { url: "https://www.amd.com/content/dam/amd/en/documents/instinct-business-docs/white-papers/amd-cdna-white-paper.pdf", title: "AMD CDNA Architecture white paper", trust: 0.95 }
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi100.html", title: "AMD Instinct MI100 specifications", trust: 0.95 }
  - { url: "https://www.amd.com/en/technologies/cdna.html", title: "AMD CDNA Architecture (generation table)", trust: 0.95 }
---

## What Changed
CDNA is AMD's **compute-only** GPU architecture. Its first product, the **Instinct MI100**, launched on
16 November 2020 on TSMC 7nm with 32 GB of **HBM2** (up to 1.2 TB/s).

- **Matrix Core Engines:** added to compute units derived from GCN; they run **MFMA** instructions on
  INT8, FP16, BF16 and FP32 inputs with INT32 or FP32 output.
- **No graphics pipeline:** AMD removed rasterization, tessellation, graphics caches, blending and the
  display engine, keeping video decode.
- **Scaling:** three **Infinity Fabric** links per GPU allow fully connected four-GPU hives; the host link
  is **PCIe 4.0**.
- **Precision:** on the MI100, FP64 vector peak is half the FP32 vector peak (11.5 versus 23.1 TFLOPS).
