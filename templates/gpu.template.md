---
id: gpu/<slug>
type: gpu
slug: <slug>
schema_version: 2.2
title: "<Product name>"
vendor: NVIDIA                     # NVIDIA | AMD | Intel | Apple | Google
segment: datacenter                # datacenter | workstation | consumer
series: "<product family>"
generation: "<architecture generation>"
compute_platform: cuda              # cuda | rocm | apple-silicon | intel-gpu | intel-gaudi | google-tpu
compute_capability: <number>       # NVIDIA only, as NVIDIA lists it; absent when NVIDIA lists none
release_date: "<YYYY-MM-DD>"       # optional; maker's availability or launch date (see CONVENTIONS.md)
signal_strength: high              # high | medium | low
summary: "<one sentence>"          # optional; the Overview section repeats it
aliases: ["<other written name>"]  # optional
specifications:                    # every field but unit_kind is absent when the maker does not publish it
  unit_kind: gpu                   # gpu | module (module: several GPUs sold as one unit)
  gpus_per_module: 2               # only when unit_kind is module
  memory_gb: <number>
  memory_type: "<e.g. HBM3e>"
  memory_note: "<remark>"          # optional
  memory_kind: unified             # only when CPU and GPU share the memory
  memory_options_gb: [<number>]    # unified memory only: every size of the computers sold with the chip, smallest first
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
  basis: dense                     # optional; dense | sparse, when the maker states it
  performance_basis_note: "<what the maker says about the basis>"   # optional
ml_capabilities:                   # every field but inference is absent when no maker page supports it
  inference: true
  training: true
  fine_tuning: true
  multi_gpu_scaling:                      # optional
    technology: "<e.g. NVLink + NVSwitch>"
    max_units: <integer>                  # optional
    note: "<remark>"                      # optional
  sparsity_support: true
  transformer_engine: true
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
