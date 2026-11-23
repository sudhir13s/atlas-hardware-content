---
id: gpu/google-tpu-v5p
type: gpu
slug: google-tpu-v5p
schema_version: 3.0
title: TPU v5p
vendor: Google
segment: datacenter
series: Cloud TPU
generation: v5p
compute_platform: google-tpu
release_date: '2023-12-06'
signal_strength: high
summary: Google Cloud TPU with two TensorCores and 95 GiB of HBM at 2,765 GB/s per chip, scaling to 8,960 chips in a Pod.
aliases:
- Google TPU v5p
specifications:
  memory_gb: 95
  memory_type: HBM
  memory_bandwidth_gb_per_s: 2765
  unit_kind: gpu
  compute_units: 2
  compute_unit_type: TensorCores
  compute_unit_note: four matrix-multiply units (MXUs) per TensorCore; four SparseCores per chip
  interconnect:
    name: ICI
    bandwidth_gb_per_s: 1200
    note: bidirectional, per chip
performance:
  bf16_tflops: 459.0
  fp8_tflops: 459.0
  performance_basis_note: peak compute per chip as Google lists it
ml_capabilities:
  inference: true
  training: true
  fine_tuning: true
  transformer_engine: false
  multi_gpu_scaling:
    technology: ICI
    max_units: 8960
    note: up to 8960 chips per Pod
market:
  cloud_hourly_usd: 4.2
  cloud_providers:
  - name: Google Cloud
  observed_at: '2026-06-15'
  source: snapshot
best_for:
- Training large generative AI models
key_features:
- 95 GiB HBM per chip, 2765 GBps
- 459 TFLOPs bf16 and fp8 per chip
- 1200 GBps bidirectional ICI per chip
- Up to 8960 chips per Pod
notable_users:
- Google DeepMind
- Google Research
- Salesforce
- Lightricks
image: /images/gpus/google-tpu-v5p.png
tags:
- google
- datacenter
- v5p
updated: '2026-11-22'
sources:
- url: https://docs.cloud.google.com/tpu/docs/v5p
  title: TPU v5p (Google Cloud documentation)
  trust: 0.95
- url: https://cloud.google.com/blog/products/ai-machine-learning/introducing-cloud-tpu-v5p-and-ai-hypercomputer
  title: Introducing Cloud TPU v5p and AI Hypercomputer (Google Cloud Blog)
  trust: 0.95
- url: https://cloud.google.com/blog/products/compute/whats-new-with-google-clouds-ai-hypercomputer-architecture
  title: What's new with Google Cloud's AI Hypercomputer architecture (Google Cloud Blog)
  trust: 0.95
---


