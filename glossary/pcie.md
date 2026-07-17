---
id: glossary-term/pcie
type: glossary-term
slug: pcie
schema_version: 1.0
title: "PCIe (PCI Express)"
term: "PCIe (PCI Express)"
category: interconnect
examples: ["PCIe 4.0 x16 on Ampere/RDNA 2", "PCIe 5.0 on Hopper and MI300X", "PCIe 6.0 on Blackwell"]
related: [glossary-term/nvlink]
tags: [interconnect, pcie, host]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/PCI_Express", title: "PCI Express — Wikipedia", trust: 0.8 }
---

## Definition
PCIe is the standard serial bus that connects a GPU to the host CPU and system memory. Bandwidth doubles
roughly each generation (PCIe 4.0 ≈ 32 GB/s bidirectional over x16, 5.0 ≈ 64 GB/s, 6.0 ≈ 128 GB/s). Every
GPU speaks PCIe even when it also has NVLink or Infinity Fabric.

## Why You Care
PCIe is how data gets from CPU/storage into the GPU and how GPUs without NVLink talk to each other. It is
much slower than NVLink, so for multi-GPU training a PCIe-only setup bottlenecks on inter-GPU
communication. For single-GPU inference it matters mainly for loading weights and streaming inputs; the
generation (4.0 vs 5.0) rarely limits steady-state token generation.
