---
id: gpu/nvidia-l40
type: gpu
slug: nvidia-l40
schema_version: 3.0
title: L40
vendor: NVIDIA
segment: datacenter
generation: Ada Lovelace
architecture: gpu-architecture/ada-lovelace
compute_platform: cuda
compute_capability: 8.9
release_date: '2022-09-20'
signal_strength: low
summary: NVIDIA datacenter GPU on the Ada Lovelace architecture with 48 GB of GDDR6 with ECC at 864 GB/s in a 300 W dual-slot PCIe card.
aliases:
- NVIDIA L40
specifications:
  memory_gb: 48
  memory_type: GDDR6
  memory_bandwidth_gb_per_s: 864
  unit_kind: gpu
  compute_units: 18176
  compute_unit_type: CUDA Cores
  tensor_cores: 568
  rt_cores: 142
  tdp_watts: 300
  form_factor:
  - PCIe
  pcie_gen: 4.0
  process_node:
    nodes_nm:
    - 4
    note: TSMC 4N
performance:
  fp32_tflops: 90.5
  fp16_tflops: 181.05
  bf16_tflops: 181.05
  tf32_tflops: 90.5
  fp8_tflops: 362.0
  int8_tops: 362.0
  basis: dense
  performance_basis_note: dense; with sparsity NVIDIA lists TF32 181, FP16/BF16 362.1, FP8 724 TFLOPS and INT8 724 TOPS
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  sparsity_support: true
  transformer_engine: true
market:
  cloud_hourly_usd: 1.0
  observed_at: '2026-11-20'
  source: snapshot; GetDeploying GPU cloud prices
best_for:
- NVIDIA Omniverse Enterprise
- Rendering and 3D graphics
- Virtual workstations (NVIDIA RTX vWS)
- AI training and data science
- Streaming and video content
key_features:
- 48 GB GDDR6 with ECC, 864 GB/s
- 142 third-generation RT Cores
- 568 fourth-generation Tensor Cores
- 3 NVENC and 3 NVDEC engines with AV1 encode and decode
limitations:
- No NVLink support
- No MIG support
notable_users:
- D-ID
- Seyhan Lee
image: /images/gpus/nvidia-l40.jpg
tags:
- nvidia
- datacenter
- ada-lovelace
updated: '2026-11-22'
sources:
- url: https://www.nvidia.com/en-us/data-center/l40/
  title: NVIDIA L40 GPU (NVIDIA)
  trust: 0.95
- url: https://images.nvidia.com/content/Solutions/data-center/vgpu-L40-datasheet.pdf
  title: NVIDIA L40 datasheet (NVIDIA)
  trust: 0.95
- url: https://images.nvidia.com/aem-dam/Solutions/geforce/ada/nvidia-ada-gpu-architecture.pdf
  title: NVIDIA Ada GPU Architecture whitepaper (NVIDIA)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-announces-ovx-computing-systems-the-graphics-and-simulation-foundation-for-the-metaverse-powered-by-ada-lovelace-gpu
  title: NVIDIA Announces OVX Computing Systems Powered by Ada Lovelace GPU (NVIDIA Newsroom)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-launches-inference-platforms-for-large-language-models-and-generative-ai-workloads
  title: NVIDIA Launches Inference Platforms for Large Language Models and Generative AI Workloads (NVIDIA Newsroom)
  trust: 0.95
- url: https://getdeploying.com/dataset/gpu-prices/weekly.csv
  title: GetDeploying open datasets (getdeploying.com/dataset), CC BY 4.0; credit GetDeploying and link to the CC BY 4.0 licence.
- url: https://developer.nvidia.com/cuda-gpus
  title: CUDA GPU Compute Capability (NVIDIA)
  trust: 0.95
---


