---
id: glossary-term/process-node
type: glossary-term
slug: process-node
schema_version: 1.0
title: "Process Node"
term: "Process Node"
category: packaging
examples: ["TSMC 4N (H100)", "TSMC 4NP (Blackwell)", "TSMC 5nm | 6nm FinFET (Instinct MI300X)", "TSMC N6 (Arc A770)"]
related: [glossary-term/die-size]
tags: [packaging, process-node, fabrication]
updated: '2026-11-21'
sources:
  - { url: "https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/", title: "NVIDIA Hopper Architecture In-Depth (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/", title: "NVIDIA Blackwell Architecture (NVIDIA)", trust: 0.95 }
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html", title: "AMD Instinct MI300X Accelerators (AMD)", trust: 0.95 }
  - { url: "https://www.intel.com/content/www/us/en/products/sku/229151/intel-arc-a770-graphics-16gb/specifications.html", title: "Intel Arc A770 Graphics (16GB) specifications (Intel)", trust: 0.95 }
  - { url: "https://www.amd.com/en/technologies/rdna.html", title: "AMD RDNA Architecture (AMD)", trust: 0.95 }
---

## Definition
A process node names the manufacturing technology a chip is fabricated on, as the maker states it:
NVIDIA gives "TSMC 4N process customized for NVIDIA" for H100 and "custom-built TSMC 4NP" for
Blackwell.

## Why You Care
The node is part of what changes between generations; AMD's RDNA table moves from 7nm (RDNA) to
5~6nm (RDNA 3). A chip can also mix nodes: AMD lists the Instinct MI300X on TSMC 5nm and 6nm FinFET.
