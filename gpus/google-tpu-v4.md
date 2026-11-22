---
id: gpu/google-tpu-v4
type: gpu
slug: google-tpu-v4
schema_version: 2.0
title: TPU v4
vendor: Google
segment: datacenter
series: Cloud TPU
generation: v4
compute_platform: google-tpu
release_date: '2022-05-11'
signal_strength: high
summary: Google Cloud TPU with two TensorCores and 32 GiB of HBM2 at 1,200 GB/s per chip, scaling to 4,096 chips in a Pod.
aliases:
- Google TPU v4
specifications:
  memory_gb: 32
  memory_type: HBM2
  memory_bandwidth_gb_per_s: 1200
  unit_kind: gpu
  compute_units: 2
  compute_unit_type: TensorCores
  compute_unit_note: four matrix-multiply units (MXUs) per TensorCore
  tdp_watts: 192
  interconnect:
    name: ICI
    note: six interconnect links per chip, 3D mesh
performance:
  bf16_tflops: 275.0
  int8_tops: 275.0
  performance_basis_note: Google lists peak compute per chip as 275 teraflops (bf16 or int8)
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: ICI
    max_units: 4096
    note: up to 4096 chips in a Pod
market:
  cloud_hourly_usd: 3.22
  cloud_providers:
  - name: Google Cloud
  observed_at: '2026-06-15'
  source: snapshot
key_features:
- 32 GiB HBM2 per chip, 1200 GBps
- 275 peak teraflops (bf16 or int8) per chip
- Up to 4096 chips per Pod
- Six inter-chip interconnect links per chip
notable_users:
- Google Research
- Cohere
- LG AI Research
- Meta AI
- Salesforce Research
image: /images/gpus/google-tpu-v4.png
tags:
- google
- datacenter
- v4
updated: '2026-11-22'
sources:
- url: https://docs.cloud.google.com/tpu/docs/v4
  title: TPU v4 (Google Cloud documentation)
  trust: 0.95
- url: https://cloud.google.com/blog/products/compute/google-unveils-worlds-largest-publicly-available-ml-cluster
  title: Google unveils world's largest publicly available ML cluster (Google Cloud Blog)
  trust: 0.95
---

## Overview

Google Cloud TPU with two TensorCores and 32 GiB of HBM2 at 1,200 GB/s per chip, scaling to 4,096 chips in a Pod.
