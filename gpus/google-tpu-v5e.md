---
id: gpu/google-tpu-v5e
type: gpu
slug: google-tpu-v5e
schema_version: 3.0
title: TPU v5e
vendor: Google
segment: datacenter
series: Cloud TPU
generation: v5e
compute_platform: google-tpu
release_date: '2023-08-29'
signal_strength: medium
summary: Google Cloud TPU with one TensorCore and 16 GiB of HBM at 819 GB/s per chip, offered for both training and inference.
aliases:
- Google TPU v5e
specifications:
  memory_gb: 16
  memory_type: HBM
  memory_bandwidth_gb_per_s: 819
  unit_kind: gpu
  compute_units: 1
  compute_unit_type: TensorCores
  compute_unit_note: four matrix-multiply units (MXUs) per TensorCore
  interconnect:
    name: ICI
    bandwidth_gb_per_s: 400
    note: bidirectional, per chip
performance:
  bf16_tflops: 197.0
  int8_tops: 393.0
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
  cloud_hourly_usd: 1.2
  cloud_providers:
  - name: Google Cloud
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Training and inference (serving)
key_features:
- 16 GiB HBM per chip, 819 GBps
- 197 TFLOPs bf16, 393 TOPs int8 per chip
- 400 GBps bidirectional ICI per chip
- Up to 256 chips per Pod
notable_users:
- Anthropic
- Hugging Face
- AssemblyAI
image: /images/gpus/google-tpu-v5e.png
tags:
- google
- datacenter
- v5e
updated: '2026-11-22'
sources:
- url: https://docs.cloud.google.com/tpu/docs/v5e
  title: TPU v5e (Google Cloud documentation)
  trust: 0.95
- url: https://cloud.google.com/blog/topics/google-cloud-next/welcome-to-google-cloud-next-23
  title: Welcome to Google Cloud Next '23 (Google Cloud Blog)
  trust: 0.95
- url: https://cloud.google.com/blog/products/compute/announcing-cloud-tpu-v5e-in-ga
  title: Announcing Cloud TPU v5e GA for cost-efficient AI model training and inference (Google Cloud Blog)
  trust: 0.95
---


