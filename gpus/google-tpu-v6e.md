---
id: gpu/google-tpu-v6e
type: gpu
slug: google-tpu-v6e
schema_version: 2.0
title: TPU v6e (Trillium)
vendor: Google
segment: datacenter
series: Cloud TPU
generation: v6e (Trillium)
compute_platform: google-tpu
release_date: '2024-12-11'
signal_strength: high
summary: Google Cloud TPU (Trillium) with one TensorCore and 32 GB of HBM at 1,638 GB/s per chip, scaling to 256 chips in a Pod.
aliases:
- Google TPU v6e (Trillium)
specifications:
  memory_gb: 32
  memory_type: HBM
  memory_bandwidth_gb_per_s: 1638
  unit_kind: gpu
  compute_units: 1
  compute_unit_type: TensorCores
  compute_unit_note: two 256x256 matrix-multiply units (MXUs) per TensorCore
  interconnect:
    name: ICI
    bandwidth_gb_per_s: 800
    note: bidirectional, per chip
performance:
  bf16_tflops: 918.0
  int8_tops: 1836.0
  performance_basis_note: peak compute per chip as Google lists it
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: ICI
    max_units: 256
    note: up to 256 chips per Pod
market:
  cloud_hourly_usd: 1.5
  cloud_providers:
  - name: Google Cloud
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Transformer, text-to-image and CNN training, fine-tuning and serving
key_features:
- 32 GB HBM per chip, 1638 GBps
- 918 TFLOPs bf16, 1836 TOPs int8 per chip
- 800 GBps bidirectional ICI per chip
- Third-generation SparseCore
notable_users:
- Deep Genomics
- HubX
- Lightricks
image: /images/gpus/google-tpu-v6e.png
tags:
- google
- datacenter
- v6e-trillium
updated: '2026-11-22'
sources:
- url: https://docs.cloud.google.com/tpu/docs/v6e
  title: TPU v6e (Google Cloud documentation)
  trust: 0.95
- url: https://cloud.google.com/blog/products/compute/introducing-trillium-6th-gen-tpus
  title: Introducing Trillium, sixth-generation TPUs (Google Cloud Blog)
  trust: 0.95
- url: https://cloud.google.com/blog/products/compute/trillium-sixth-generation-tpu-is-in-preview
  title: Trillium sixth-generation TPU is in preview (Google Cloud Blog)
  trust: 0.95
- url: https://cloud.google.com/blog/products/compute/trillium-tpu-is-ga
  title: Announcing the general availability of Trillium, our sixth-generation TPU (Google Cloud Blog)
  trust: 0.95
---

## Overview

Google Cloud TPU (Trillium) with one TensorCore and 32 GB of HBM at 1,638 GB/s per chip, scaling to 256 chips in a Pod.
