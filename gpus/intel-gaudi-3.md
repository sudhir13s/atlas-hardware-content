---
id: gpu/intel-gaudi-3
type: gpu
slug: intel-gaudi-3
schema_version: 3.0
title: Gaudi 3
vendor: Intel
segment: datacenter
series: Gaudi
generation: Gaudi 3
compute_platform: intel-gaudi
release_date: '2024-09-24'
signal_strength: medium
summary: Intel AI accelerator with 128 GB of HBM2e at 3.7 TB/s, 64 Tensor Processor Cores, 8 matrix engines and 24 integrated 200 GbE ports, in a 900 W OAM module.
aliases:
- Intel Gaudi 3
specifications:
  memory_gb: 128
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 3700
  unit_kind: gpu
  compute_units: 64
  compute_unit_type: Tensor Processor Cores (TPC)
  tdp_watts: 900
  form_factor:
  - OAM
  pcie_gen: 5.0
  interconnect:
    name: 24x 200GbE RoCE
    bandwidth_gb_per_s: 1200
    note: bidirectional
  process_node:
    nodes_nm:
    - 5
    note: TSMC 5nm
performance:
  bf16_tflops: 1678.0
  fp8_tflops: 1678.0
  performance_basis_note: Intel lists these as matrix engine (MME) TFLOPS in its current white paper; earlier Intel material listed 1835.
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: Ethernet-based
    note: RoCE; 21 ports connect the 8 OAMs of a baseboard all-to-all, 3 ports scale out
market:
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Generative AI training
- Generative AI inference
key_features:
- 128 GB HBM2e, 3.7 TB/s
- 64 Tensor Processor Cores and 8 matrix engines
- 24 x 200GbE RoCE ports on chip
- PCIe Gen5 x16 host interface
- Also offered as the HL-338 PCIe card (600 W)
notable_users:
- IBM Cloud
image: /images/gpus/intel-gaudi-3.jpg
tags:
- intel
- datacenter
- gaudi-3
updated: '2026-11-22'
sources:
- url: https://cdrdv2-public.intel.com/817486/gaudi-3-ai-accelerator-white-paper.pdf
  title: Intel Gaudi 3 AI Accelerator White Paper (Intel)
  trust: 0.95
- url: https://cdrdv2-public.intel.com/845118/gaudi-3-ai-accelerator-30-3-30.pdf
  title: Intel Gaudi 3 AI Accelerator overview (Intel)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/content-details/817487/intel-gaudi-3-ai-accelerator-325-l-oam-mezzanine-card-product-brief.html
  title: Intel Gaudi 3 AI Accelerator 325-L OAM Mezzanine Card Product Brief (Intel)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/products/details/processors/ai-accelerators/gaudi.html
  title: Intel Gaudi 3 AI Accelerators (Intel)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/newsroom/news/vision-2024-gaudi-3-ai-accelerator.html
  title: Intel Breaks Down Proprietary Walls to Bring Choice to Enterprise GenAI Market (Intel)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/newsroom/news/next-generation-ai-solutions-xeon-6-gaudi-3.html
  title: Intel Unveils Next-Generation AI Solutions with the Launch of Xeon 6 and Gaudi 3 (Intel)
  trust: 0.95
---


