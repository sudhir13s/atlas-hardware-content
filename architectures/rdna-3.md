---
id: gpu-architecture/rdna-3
type: gpu-architecture
slug: rdna-3
schema_version: 3.0
title: AMD RDNA 3
name: RDNA 3
vendor: AMD
year: 2022
predecessors:
- gpu-architecture/rdna-2
process_node: TSMC 5nm (GCD) + 6nm (MCD)
segment: consumer
representative_gpus:
- gpu/amd-rx-7900-xtx
key_innovation: 'A chiplet design: a 5nm Graphics Compute Die with 6nm Memory Cache Dies, plus AI accelerators in the compute units.'
innovations:
- 'Chiplet design: 5nm Graphics Compute Die (GCD) + six 6nm Memory Cache Dies (MCD)'
- AI accelerators (1st generation)
- Ray Accelerators (2nd generation)
- AMD Infinity Cache (2nd generation)
- AMD Radiance Display Engine with DisplayPort 2.1
precision_support:
- FP32
- FP16
- BF16
- INT8
- INT4
memory_tech: GDDR6
interconnect: PCIe 4.0
tags:
- amd
- rdna-3
- chiplet
updated: '2026-11-21'
sources:
- url: https://ir.amd.com/news-events/press-releases/detail/1099/amd-unveils-worlds-most-advanced-gaming-graphics-cards-built-on-groundbreaking-amd-rdna-3-architecture-with-chiplet-design
  title: 'AMD press release: Radeon RX 7900 Series unveiled (3 November 2022)'
  trust: 0.95
- url: https://www.amd.com/en/products/graphics/desktops/radeon/7000-series/amd-radeon-rx-7900xtx.html
  title: AMD Radeon RX 7900 XTX specifications
  trust: 0.95
- url: https://www.amd.com/en/products/graphics/workstations/radeon-pro/w7900.html
  title: AMD Radeon PRO W7900 specifications (RDNA 3, TSMC 5nm GCD / 6nm MCD, PCIe 4.0 x16)
  trust: 0.95
- url: https://www.amd.com/en/technologies/rdna.html
  title: AMD RDNA Architecture (generation table)
  trust: 0.95
---

## What Changed

RDNA 3 arrived with the **Radeon RX 7900 XTX** and **RX 7900 XT**, unveiled on 3 November 2022 and
available from 13 December 2022.

- **Chiplets:** one **5nm Graphics Compute Die (GCD)** with up to 96 compute units, plus six **6nm
  Memory Cache Dies (MCD)**, each with up to 16 MB of Infinity Cache. AMD calls these the first gaming
  graphics cards with a chiplet design.
- **AI accelerators:** AMD's first generation in a gaming GPU. The RX 7900 XTX lists FP16, INT8 and
  INT4 matrix throughput, and AMD cites BF16 rates.
- **Ray tracing:** second-generation Ray Accelerators, which AMD says are up to 1.8x faster than RDNA 2.
- **Efficiency:** AMD claims up to 54% more performance per watt than RDNA 2.
- **Display:** the AMD Radiance Display Engine supports DisplayPort 2.1 and HDMI 2.1a.
