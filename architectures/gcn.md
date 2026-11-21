---
id: gpu-architecture/gcn
type: gpu-architecture
slug: gcn
schema_version: 1.0
title: "AMD GCN (Graphics Core Next)"
name: "Graphics Core Next"
vendor: AMD
year: 2011
successor: gpu-architecture/rdna
process_node: "28nm (Radeon HD 7970)"
segment: "consumer + workstation"
representative_gpus: []
key_innovation: "Compute units that pair a scalar execution unit with vector execution units, launched as a GPU design for both gaming and compute."
innovations: ["Scalar unit plus four vector units per compute unit", "28nm production (Radeon HD 7970)", "PCI Express 3.0 (Radeon HD 7970)"]
precision_support: ["FP32"]
memory_tech: "GDDR5 (Radeon HD 7970)"
interconnect: "PCIe 3.0"
tags: [amd, gcn, compute]
updated: '2026-11-21'
sources:
  - { url: "https://ir.amd.com/news-events/press-releases/detail/201/amd-launches-worlds-fastest-single-gpu-graphics-card----the-amd-radeontm-hd-7970", title: "AMD press release: AMD Radeon HD 7970 launch (22 December 2011)", trust: 0.95 }
  - { url: "https://ir.amd.com/news-events/press-releases/detail/744/vega-amds-new-graphics-architecture-for-virtually-unlimited-workloads", title: "AMD press release: Vega architecture preview (5 January 2017), footnote on GCN-based Radeon and FirePro GPUs", trust: 0.95 }
  - { url: "https://www.amd.com/content/dam/amd/en/documents/instinct-business-docs/white-papers/amd-cdna-white-paper.pdf", title: "AMD CDNA Architecture white paper (GCN compute unit background)", trust: 0.95 }
  - { url: "https://gpuopen.com/download/RDNA_Architecture_public.pdf", title: "AMD GPUOpen: RDNA Architecture presentation (GCN comparison)", trust: 0.95 }
---

## What Changed
Graphics Core Next (GCN) arrived with the **Radeon HD 7970**, which AMD launched on 22 December 2011
(retail availability 9 January 2012). AMD built it on **28nm** with **GDDR5** memory and **PCI
Express 3.0**, and said the architecture enabled "new levels of gaming and compute capabilities".

- **Compute unit:** AMD describes the classic GCN compute unit as a scalar execution unit with its own
  register file and cache, plus four vector execution units optimized for FP32.
- **Products:** AMD's footnotes name both Radeon and FirePro GPUs as GCN-based.
- **Successors:** AMD later split the line in two. **RDNA** is optimized for gaming and **CDNA** for
  compute; AMD states CDNA's compute units are derived from GCN.
