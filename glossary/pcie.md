---
id: glossary-term/pcie
type: glossary-term
slug: pcie
schema_version: 1.0
title: "PCIe (PCI Express)"
term: "PCIe (PCI Express)"
category: interconnect
examples: ["PCI Express Gen 4 on GeForce RTX 3090 and RTX 4090", "PCIe Gen5 (128 GB/s) on H100 SXM", "PCIe 5.0 x16 on Instinct MI300X"]
related: [glossary-term/nvlink]
tags: [interconnect, pcie, host]
updated: '2026-11-21'
sources:
  - { url: "https://pcisig.com/faq?field_category_value%5B%5D=pci_express_4.0", title: "PCI Express 4.0 FAQ (PCI-SIG)", trust: 0.95 }
  - { url: "https://pcisig.com/faq?field_category_value%5B%5D=pci_express_5.0", title: "PCI Express 5.0 FAQ (PCI-SIG)", trust: 0.95 }
  - { url: "https://pcisig.com/faq?field_category_value%5B%5D=pci_express_6.0", title: "PCI Express 6.0 FAQ (PCI-SIG)", trust: 0.95 }
  - { url: "https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/", title: "NVIDIA Hopper Architecture In-Depth (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/geforce/graphics-cards/30-series/rtx-3090-3090ti/", title: "GeForce RTX 3090 specifications (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/", title: "GeForce RTX 4090 specifications (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/h100/", title: "NVIDIA H100 Tensor Core GPU (NVIDIA)", trust: 0.95 }
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html", title: "AMD Instinct MI300X Accelerators (AMD)", trust: 0.95 }
---

## Definition
PCIe is the standard serial bus that connects a GPU to the host CPU. PCI-SIG doubles the bit rate each
generation: 16.0 GT/s (4.0), 32.0 GT/s (5.0), 64.0 GT/s (6.0). Over x16, PCI-SIG gives 128.0 GB/s for
5.0 and 256.0 GB/s bidirectional for 6.0.

## Why You Care
PCIe carries data from the CPU and storage into the GPU, and between GPUs that lack a faster link.
NVIDIA lists H100 SXM at 128 GB/s over PCIe Gen5 (64 GB/s each direction) against 900 GB/s over NVLink.
