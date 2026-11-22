---
id: gpu/nvidia-t4
type: gpu
slug: nvidia-t4
schema_version: 2.0
title: T4
vendor: NVIDIA
segment: datacenter
series: Turing
generation: Turing
compute_platform: cuda
compute_capability: 7.5
release_date: '2018-09-12'
signal_strength: low
summary: NVIDIA datacenter GPU on the Turing architecture with 16 GB of GDDR6 at 320 GB/s in a 70 W low-profile PCIe card.
aliases:
- NVIDIA T4
specifications:
  memory_gb: 16
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 320
  unit_kind: gpu
  compute_units: 2560
  compute_unit_type: CUDA Cores
  tensor_cores: 320
  tdp_watts: 70
  form_factor:
  - PCIe (low-profile)
  pcie_gen: 3.0
  process_node:
    nodes_nm:
    - 12
    note: TSMC 12 nm FFN
performance:
  fp32_tflops: 8.1
  fp16_tflops: 65.0
  int8_tops: 130.0
  performance_basis_note: FP16 is NVIDIA's mixed-precision (FP16/FP32) Tensor Core figure; NVIDIA also lists 260 INT4 TOPS
ml_capabilities:
  inference: true
  training: true
  sparsity_support: false
  transformer_engine: false
market:
  cloud_hourly_usd: 0.752
  cloud_providers:
  - name: AWS
    instance_note: g4dn
  - name: GCP
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- Deep learning inference and training
- Video transcoding
- Virtual desktops
key_features:
- 16 GB GDDR6, 320 GB/s
- 70 W, single-slot low-profile PCIe card
- 320 Turing Tensor Cores
- INT8 and INT4 precision
notable_users:
- Google Cloud Platform
- Baidu
- Tencent
- JD.com
- iFLYTEK
image: /images/gpus/nvidia-t4.jpg
tags:
- nvidia
- datacenter
- turing
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/en-us/data-center/tesla-t4/
  title: NVIDIA T4 Tensor Core GPU (NVIDIA)
  trust: 0.95
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/tesla-t4/t4-tensor-core-product-brief.pdf
  title: NVIDIA T4 70W Low Profile PCIe GPU Accelerator product brief (NVIDIA)
  trust: 0.95
- url: https://images.nvidia.com/aem-dam/Solutions/design-visualization/technologies/turing-architecture/NVIDIA-Turing-Architecture-Whitepaper.pdf
  title: NVIDIA Turing GPU Architecture whitepaper (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/new-nvidia-data-center-inference-platform-to-fuel-next-wave-of-ai-powered-services
  title: New NVIDIA Data Center Inference Platform to Fuel Next Wave of AI-Powered Services (NVIDIA Newsroom)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-turing-t4-cloud-gpu-adoption-accelerates
  title: NVIDIA Turing T4 Cloud GPU Adoption Accelerates (NVIDIA Newsroom)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---

## Overview

NVIDIA datacenter GPU on the Turing architecture with 16 GB of GDDR6 at 320 GB/s in a 70 W low-profile PCIe card.
