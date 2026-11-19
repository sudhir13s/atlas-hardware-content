---
id: gpu/intel-gaudi-2
type: gpu
slug: intel-gaudi-2
schema_version: 1.1
title: Gaudi 2
vendor: Intel
segment: datacenter
series: Gaudi
generation: Gaudi 2
release_date: '2022-05-31'
signal_strength: medium
summary: Intel's AI training accelerator with 96GB HBM2e and unique Ethernet-based scaling, offering NVIDIA alternative.
aliases:
- Intel Gaudi 2
specifications:
  memory_gb: 96
  memory_type: HBM2e
  memory_bandwidth_gb_per_s: 2460
  unit_kind: gpu
  compute_units: 24
  compute_unit_type: Tensor Processor Cores (TPC)
  tdp_watts: 600
  form_factor:
  - OAM
  - PCIe
  pcie_gen: 4.0
  interconnect:
    name: 24x 100GbE RoCE RDMA
  process_node:
    nodes_nm:
    - 7
performance:
  fp32_tflops: 45.0
  fp16_tflops: 432.0
  bf16_tflops: 432.0
  fp8_tflops: 865.0
  int8_tops: 865.0
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: 40
  max_model_params_b_training: 15
  sparsity_support: false
  transformer_engine: false
  multi_gpu_scaling:
    technology: Ethernet-based
    note: RoCE RDMA
framework_support:
  pytorch: true
  tensorflow: true
  jax: false
  onnx_runtime: false
  tensorrt: false
  directml: false
  mlx: false
  rocm: false
  oneapi: true
  triton: false
  vllm: true
  deepspeed: true
market:
  cloud_hourly_usd: 1.7
  cloud_providers:
  - name: AWS
    instance_note: dl2q instances
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Cost-effective training alternative
- LLM fine-tuning
- Multi-node training via Ethernet
key_features:
- 96 GB HBM2e
- Integrated 24x 100GbE for multi-card scaling
- FP8 support
- Habana SynapseAI software stack
limitations:
- Smaller software ecosystem
- Less community support
- Fewer framework integrations
notable_users:
- AWS (dl2q)
- Intel AI labs
image: /images/gpus/intel-gaudi-2.jpg
tags:
- intel
- datacenter
- gaudi-2
updated: '2026-11-19'
sources: []
---

## Overview

Intel's AI training accelerator with 96GB HBM2e and unique Ethernet-based scaling, offering NVIDIA alternative.
