---
id: glossary-term/die-size
type: glossary-term
slug: die-size
schema_version: 1.0
title: "Die Size and Reticle Limit"
term: "Die Size and Reticle Limit"
category: packaging
examples: ["814 mm² GH100 (Hopper)", "Blackwell: two reticle-limited dies joined by a 10 TB/s chip-to-chip interconnect", "Instinct MI300X: 8 CDNA 3 compute-die chiplets"]
related: [glossary-term/process-node]
tags: [packaging, die-size, chiplet]
updated: '2026-11-21'
sources:
  - { url: "https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/", title: "NVIDIA Hopper Architecture In-Depth (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/", title: "NVIDIA Blackwell Architecture (NVIDIA)", trust: 0.95 }
  - { url: "https://3dfabric.tsmc.com/english/dedicatedFoundry/technology/cowos.htm", title: "CoWoS (TSMC 3DFabric)", trust: 0.95 }
  - { url: "https://www.amd.com/en/technologies/cdna.html", title: "AMD CDNA Architecture (AMD)", trust: 0.95 }
  - { url: "https://www.amd.com/en/technologies/rdna.html", title: "AMD RDNA Architecture (AMD)", trust: 0.95 }
---

## Definition
Die size is the physical area of one chip; NVIDIA gives 814 mm² for the GH100 die. The reticle is the
area patterned in one lithography exposure. TSMC gives 3.3 reticles as about 2,700 mm², so one reticle
is about 820 mm² by that arithmetic.

## Why You Care
A single die cannot exceed one reticle, so larger designs combine several dies in one package.
NVIDIA describes Blackwell GPUs as two reticle-limited dies; AMD builds the Instinct MI300X from eight
compute-die chiplets and describes RDNA 3 as a chiplet design.
