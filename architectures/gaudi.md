---
id: gpu-architecture/gaudi
type: gpu-architecture
slug: gaudi
schema_version: 3.0
title: Intel Gaudi (Habana)
name: Gaudi
vendor: Intel
codename: Gaudi / Gaudi 2 / Gaudi 3
year: 2019
process_node: 16nm (Gaudi) → 7nm (Gaudi 2) → TSMC 5nm (Gaudi 3)
segment: datacenter
representative_gpus:
- gpu/intel-gaudi-2
- gpu/intel-gaudi-3
key_innovation: A deep-learning accelerator (not a GPU) built from Matrix Multiplication Engines and programmable Tensor Processor Cores, with RDMA over Converged Ethernet (RoCE) ports integrated on the chip.
innovations:
- Matrix Multiplication Engine (MME) + programmable Tensor Processor Cores (TPC)
- 'Integrated RoCE v2 Ethernet ports on chip: 10 (Gaudi), 24 x 100 GbE (Gaudi 2), 24 x 200 GbE (Gaudi 3)'
- FP8 introduced with Gaudi 2
- 'HBM memory: 32 GB HBM2 (Gaudi), 96 GB HBM2E (Gaudi 2), 128 GB HBM2e (Gaudi 3)'
precision_support:
- FP32
- TF32 (Gaudi 3)
- BF16
- FP16
- FP8 (Gaudi 2, Gaudi 3)
- INT8
memory_tech: HBM2 (Gaudi) → HBM2E (Gaudi 2, Gaudi 3)
interconnect: Integrated RoCE v2 Ethernet; PCIe Gen4 (Gaudi 2), PCIe Gen5 (Gaudi 3)
tags:
- intel
- gaudi
- habana
- accelerator
- ethernet
updated: '2026-11-21'
sources:
- url: https://download.intel.com/newsroom/2021/archive/2019-12-16-news-releases-intel-ai-acquisition.pdf
  title: 'Intel news release: Intel Acquires Artificial Intelligence Chipmaker Habana Labs (16 December 2019)'
  trust: 0.95
- url: https://download.intel.com/newsroom/2022/corporate/vision/Habana-Gaudi2-Launch-Fact-Sheet.pdf
  title: 'Intel fact sheet: Habana Labs Launches Gaudi2 (10 May 2022)'
  trust: 0.95
- url: https://download.intel.com/newsroom/archive/2025/en-us-2021-11-16-intels-habana-labs-announces-turnkey-ai-training-solution.pdf
  title: 'Intel Newsroom: Habana Labs turnkey AI training solution (32 GB HBM2 per Gaudi)'
  trust: 0.95
- url: https://cdrdv2-public.intel.com/817486/gaudi-3-ai-accelerator-white-paper.pdf
  title: Intel Gaudi 3 AI Accelerator technical paper
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/newsroom/news/next-generation-ai-solutions-xeon-6-gaudi-3.html
  title: 'Intel Newsroom: launch of Xeon 6 and Gaudi 3 (24 September 2024)'
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/products/details/processors/ai-accelerators/gaudi.html
  title: Intel Gaudi AI Accelerator products
  trust: 0.95
---

## What Changed

Gaudi comes from **Habana Labs**, which Intel acquired on 16 December 2019 while the first Gaudi
training processor was sampling. It is a deep-learning accelerator rather than a GPU.

- **Compute:** a **Matrix Multiplication Engine** handles matrix operations; programmable **Tensor
  Processor Cores** (a VLIW SIMD processor) handle the rest.
- **Networking:** RoCE Ethernet ports sit on the chip, so systems scale up and out over standard
  Ethernet switches. Intel positions this as an open alternative to proprietary fabrics such as NVLink.
- **Gaudi 2** (launched 10 May 2022): 7nm (from 16nm), FP8 added, 24 Tensor Processor Cores (from 8),
  96 GB HBM2E at 2.45 TB/s, and 24 integrated 100 GbE RoCE ports.
- **Gaudi 3** (launched 24 September 2024): TSMC 5nm, 8 MMEs and 64 TPCs, 128 GB HBM2e at 3.7 TB/s,
  24 x 200 GbE RoCE and a PCIe Gen5 host link.
