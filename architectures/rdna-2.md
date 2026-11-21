---
id: gpu-architecture/rdna-2
type: gpu-architecture
slug: rdna-2
schema_version: 1.0
title: "AMD RDNA 2"
name: "RDNA 2"
vendor: AMD
year: 2020
predecessor: gpu-architecture/rdna
successor: gpu-architecture/rdna-3
process_node: "7nm (6nm on some later models)"
segment: "consumer"
representative_gpus: []
key_innovation: "AMD Infinity Cache, a large on-die last-level cache, plus a fixed-function Ray Accelerator in each compute unit."
innovations: ["AMD Infinity Cache (1st generation, 128 MB on Radeon RX 6900 XT)", "Ray Accelerators (1st generation, one per compute unit)", "Up to 54% more performance per watt than RDNA on the same 7nm process (AMD figure, RX 6800 XT vs RX 5700 XT)", "AMD Smart Access Memory (with Ryzen 5000 Series processors)", "Foundation for the PlayStation 5 and Xbox Series S and X consoles"]
precision_support: ["FP32", "FP16"]
memory_tech: "GDDR6"
interconnect: "PCIe 4.0"
tags: [amd, rdna-2, ray-tracing, infinity-cache]
updated: '2026-11-21'
sources:
  - { url: "https://ir.amd.com/news-events/press-releases/detail/978/amd-unveils-next-generation-pc-gaming-with-amd-radeon-rx-6000-series-bringing-leadership-4k-resolution-performance-to-aaa-gaming", title: "AMD press release: Radeon RX 6000 Series unveiled (28 October 2020)", trust: 0.95 }
  - { url: "https://www.amd.com/en/products/graphics/desktops/radeon/6000-series/amd-radeon-rx-6900-xt.html", title: "AMD Radeon RX 6900 XT specifications", trust: 0.95 }
  - { url: "https://www.amd.com/en/technologies/rdna.html", title: "AMD RDNA Architecture (generation table)", trust: 0.95 }
  - { url: "https://ir.amd.com/financial-information/sec-filings/content/0000002488-22-000016/0000002488-22-000016.pdf", title: "AMD Form 10-K for fiscal 2021 (RDNA 2 in PlayStation 5 and Xbox Series S and X)", trust: 0.95 }
---

## What Changed
RDNA 2 arrived with the **Radeon RX 6000 Series**, which AMD unveiled on 28 October 2020; the RX 6800
and RX 6800 XT were due on 18 November 2020 and the RX 6900 XT on 8 December 2020.

- **Infinity Cache:** a 128 MB on-die last-level cache that AMD says reduces latency; the cards pair it
  with a 256-bit GDDR6 interface.
- **Ray tracing:** a fixed-function **Ray Accelerator** in each compute unit, AMD's first generation.
- **Efficiency:** AMD claims up to 54% more performance per watt than RDNA on the same 7nm process.
- **Consoles:** AMD's annual report calls RDNA 2 the foundation for the **PlayStation 5** and **Xbox
  Series S and X**.
- **Process:** AMD's generation table lists RDNA 2 at 6nm to 7nm.
