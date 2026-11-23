---
id: gpu-architecture/rdna
type: gpu-architecture
slug: rdna
schema_version: 3.0
title: AMD RDNA
name: RDNA
vendor: AMD
codename: Navi
year: 2019
predecessors:
- gpu-architecture/gcn
process_node: 7nm
segment: consumer
representative_gpus: []
key_innovation: A gaming-focused redesign of the GCN compute unit around the workgroup processor (two compute units sharing resources), aimed at lower latency and higher performance per clock.
innovations:
- 'Workgroup processor: resources of two compute units available to one workgroup'
- Native Wave32 execution
- New L1 cache per shader array
- GDDR6 memory
- PCIe 4.0
- Up to 1.25x performance per clock and up to 1.5x performance per watt versus GCN (AMD figures)
precision_support:
- FP32
- FP16
memory_tech: GDDR6
interconnect: PCIe 4.0
tags:
- amd
- rdna
- navi
- gaming
updated: '2026-11-21'
sources:
- url: https://ir.amd.com/news-events/press-releases/detail/899/amd-unleashes-ultimate-pc-gaming-platform-with-worldwide-availability-of-amd-radeon-rx-5700-series-graphics-cards-and-amd-ryzen-3000-series-desktop-processors
  title: 'AMD press release: Radeon RX 5700 series availability (7 July 2019)'
  trust: 0.95
- url: https://gpuopen.com/download/RDNA_Architecture_public.pdf
  title: 'AMD GPUOpen: RDNA Architecture presentation'
  trust: 0.95
- url: https://www.amd.com/en/support/downloads/drivers.html/graphics/radeon-rx/radeon-rx-5000-series/amd-radeon-rx-5700-xt.html
  title: AMD Radeon RX 5700 XT specifications
  trust: 0.95
- url: https://www.amd.com/en/technologies/rdna.html
  title: AMD RDNA Architecture (generation table)
  trust: 0.95
- url: https://www.amd.com/content/dam/amd/en/documents/instinct-business-docs/white-papers/amd-cdna-white-paper.pdf
  title: AMD CDNA Architecture white paper (RDNA and CDNA split)
  trust: 0.95
---

## What Changed

RDNA replaced GCN in AMD's **gaming** GPUs, starting with the **Radeon RX 5700 XT** and **RX 5700**
(available 7 July 2019) on **7nm** with **GDDR6** and **PCIe 4.0**.

- **Compute:** the **workgroup processor** gives one workgroup the resources of two compute units, with
  native Wave32 execution and twice the scalar resources. AMD calls GCN compute-focused and RDNA
  graphics- and latency-focused.
- **Caches:** a new L1 cache per shader array sits between the compute units and the L2.
- **Efficiency:** AMD claims up to 1.25x performance per clock and up to 1.5x performance per watt
  versus GCN.
- **Not included:** AMD's generation table starts ray-tracing accelerators at RDNA 2 and AI
  accelerators at RDNA 3.
- **Split:** with RDNA for gaming, AMD moved datacenter compute to the separate CDNA architecture.
