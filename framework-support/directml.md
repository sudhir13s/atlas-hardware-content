---
id: framework-support/directml
type: framework-support
slug: directml
schema_version: 2.0
title: DirectML
checked: '2026-11-22'
platforms:
- platform: cuda
  supported: true
  note: Windows; Microsoft states DirectML runs on all DirectX 12-compatible hardware, and these GPUs' maker pages list DirectX 12. DirectML is in sustained engineering
  gpus:
  - gpu/nvidia-rtx-3080
  - gpu/nvidia-rtx-3090
  - gpu/nvidia-rtx-4080
  - gpu/nvidia-rtx-4090
  - gpu/nvidia-rtx-5090
  - gpu/nvidia-a4000
  - gpu/nvidia-a5000
  - gpu/nvidia-a6000
  source: https://learn.microsoft.com/en-us/windows/ai/directml/dml
- platform: intel-gpu
  supported: true
  note: Windows; Intel lists DirectX 12 Ultimate for the Arc A770. DirectML is in sustained engineering
  gpus:
  - gpu/intel-arc-a770
  source: https://learn.microsoft.com/en-us/windows/ai/directml/dml
tags:
- directml
- framework-support
updated: '2026-11-22'
sources:
- url: https://learn.microsoft.com/en-us/windows/ai/directml/dml
  title: Introduction to DirectML (Microsoft Learn)
  trust: 0.95
---
