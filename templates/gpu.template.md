---
id: gpu/<slug>
type: gpu
slug: <slug>
schema_version: 1.3
title: "<Product name>"
vendor: NVIDIA                     # NVIDIA | AMD | Intel | Apple | Google
segment: datacenter                # datacenter | workstation | consumer
series: "<product family>"
generation: "<architecture generation>"
release_date: "<YYYY-MM-DD>"
signal_strength: high              # high | medium | low
summary: "<one sentence>"          # optional; the Overview section repeats it
aliases: ["<other written name>"]  # optional
specifications:
  unit_kind: gpu                   # gpu | module (module: several GPUs sold as one unit)
  gpus_per_module: 2               # only when unit_kind is module
  memory_gb: <number>
  memory_type: "<e.g. HBM3e>"
  memory_note: "<remark>"          # optional
  memory_kind: unified             # only when CPU and GPU share the memory
  memory_bandwidth_gb_per_s: <number>
  compute_units: <integer>
  compute_unit_type: "<e.g. CUDA Cores>"
  compute_unit_note: "<remark>"    # optional
  tensor_cores: <integer>          # optional; absent when the GPU has none
  rt_cores: <integer>              # optional
  tdp_watts: <number>
  form_factor: ["<e.g. SXM5>"]
  pcie_gen: <number>               # optional
  interconnect:                    # optional
    name: "<e.g. NVLink 4.0>"
    bandwidth_gb_per_s: <number>   # optional
    note: "<remark>"               # optional
  process_node:
    nodes_nm: [<number>]
    note: "<original text>"        # optional; for composite or remarked nodes
performance:                       # peak figures as the vendor gives them; absent when unpublished
  fp32_tflops: <number>
  fp16_tflops: <number>
  bf16_tflops: <number>
  tf32_tflops: <number>
  fp8_tflops: <number>
  int8_tops: <number>
  performance_basis_note: "<dense or sparse, when stated>"   # optional
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  max_model_params_b_inference: <number>
  max_model_params_b_training: <number>   # optional
  multi_gpu_scaling:                      # optional
    technology: "<e.g. NVLink + NVSwitch>"
    max_units: <integer>                  # optional
    note: "<remark>"                      # optional
  sparsity_support: true
  transformer_engine: true
framework_support:
  pytorch: true
  tensorflow: true
  jax: false
  onnx_runtime: false
  tensorrt: false
  directml: false
  mlx: false
  rocm: false
  oneapi: false
  triton: false
  vllm: false
  deepspeed: false
market:                            # agent-owned; unknown prices are absent
  msrp_usd: <number>               # optional; only the maker's own published launch price
  msrp_source: "<maker page URL>"  # optional; the page that states msrp_usd
  msrp_announced: "<YYYY-MM-DD>"   # optional; date of that announcement
  cloud_hourly_usd: <number>
  cloud_providers:
    - { name: "<provider>", instance_note: "<instance family>" }
  observed_at: "<YYYY-MM-DD>"
  source: "<where the prices came from>"
best_for: ["<label>"]
key_features: ["<label>"]
limitations: ["<label>"]
notable_users: ["<label>"]
image: "/images/gpus/<slug>.jpg"
tags: [<tag>]
updated: <YYYY-MM-DD>
sources:
  - { url: "<url>", title: "<title>", trust: 0.9 }
---

## Overview
<The summary, verbatim.>
