---
id: gpu-architecture/gaudi
type: gpu-architecture
slug: gaudi
schema_version: 1.0
title: "Intel Gaudi (Habana)"
name: "Gaudi"
vendor: Intel
codename: "Gaudi 1 / 2 / 3"
year: 2019
process_node: "TSMC 16nm (Gaudi 1) → 7nm (Gaudi 2) → 5nm (Gaudi 3)"
segment: "datacenter"
representative_gpus: ["Habana Gaudi (2019)", "Gaudi 2 (2022)", "Gaudi 3 (2024)"]
key_innovation: "A purpose-built AI training/inference accelerator (not a GPU) with RDMA-over-Converged-Ethernet ports integrated on-chip for networkless scale-out."
innovations: ["Matrix Multiplication Engine + programmable Tensor Processor Cores", "Integrated RoCE v2 Ethernet ports on-die (no separate NIC to scale out)", "HBM memory", "FP8 support (Gaudi 3)", "Open, standards-based Ethernet scale-out fabric"]
precision_support: ["BF16", "FP16", "FP8 (Gaudi 3)", "INT8"]
memory_tech: "HBM2 (Gaudi 1) → HBM2e (Gaudi 2/3)"
interconnect: "Integrated RoCE v2 Ethernet, PCIe"
tags: [intel, gaudi, habana, accelerator, ethernet]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Habana_Labs", title: "Habana Labs (Gaudi) — Wikipedia", trust: 0.8 }
  - { url: "https://www.intel.com/content/www/us/en/products/details/processors/ai-accelerators/gaudi.html", title: "Intel Gaudi AI Accelerators", trust: 0.9 }
---

## What Changed
Gaudi came from **Habana Labs**, which Intel acquired in 2019, and is an **AI accelerator rather than a
GPU** — it has no graphics pipeline at all. Its compute is built from a **Matrix Multiplication
Engine** plus programmable **Tensor Processor Cores**. Gaudi's distinctive design choice is
**integrating standards-based RoCE v2 Ethernet ports directly on the chip**: accelerators scale out
over ordinary Ethernet switches without a separate NIC or a proprietary fabric like NVLink, which Intel
positions as a lower-cost, more open path to large clusters. **Gaudi 2** (7nm, HBM2e) offered
competitive training price/performance versus A100/H100 on some workloads, and **Gaudi 3** (5nm) added
**FP8** and more HBM. Gaudi is Intel's main datacenter-AI answer, kept separate from the Xe GPU line.
