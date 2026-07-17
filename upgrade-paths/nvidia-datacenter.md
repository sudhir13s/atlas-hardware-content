---
id: upgrade-path/nvidia-datacenter
type: upgrade-path
slug: nvidia-datacenter
schema_version: 1.0
title: "NVIDIA datacenter training GPUs"
vendor: NVIDIA
family: "Datacenter (Tesla / Data Center)"
steps:
  - { gpu_id: "Tesla V100", architecture_id: gpu-architecture/volta, year: 2017 }
  - { gpu_id: "A100", architecture_id: gpu-architecture/ampere, year: 2020 }
  - { gpu_id: "H100", architecture_id: gpu-architecture/hopper, year: 2022 }
  - { gpu_id: "H200", architecture_id: gpu-architecture/hopper, year: 2023 }
  - { gpu_id: "B200", architecture_id: gpu-architecture/blackwell, year: 2024 }
tags: [nvidia, datacenter, training]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/List_of_Nvidia_graphics_processing_units", title: "List of NVIDIA GPUs — Wikipedia", trust: 0.8 }
---

## Overview
The mainline of NVIDIA datacenter training accelerators — each generation adding Tensor-Core generations,
new precisions (FP16 → TF32/BF16 → FP8 → FP4), faster memory (HBM2 → HBM2e → HBM3 → HBM3e), and higher
NVLink bandwidth. This is the sequence most large models have been trained on.
