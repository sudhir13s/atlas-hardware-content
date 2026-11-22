---
id: gpu/nvidia-b100
type: gpu
slug: nvidia-b100
schema_version: 2.0
title: B100
vendor: NVIDIA
segment: datacenter
series: Blackwell
generation: Blackwell
compute_platform: cuda
release_date: '2024-03-18'
signal_strength: high
summary: NVIDIA named the B100 Tensor Core GPU as part of its Blackwell platform on March 18, 2024, and documents an HGX B100 8-GPU baseboard with fourth-generation NVSwitches. NVIDIA publishes no specification page for the B100.
aliases:
- NVIDIA B100
specifications:
  unit_kind: gpu
performance: {}
ml_capabilities:
  inference: true
  training: true
  multi_gpu_scaling:
    technology: NVLink with fourth-generation NVSwitch (HGX B100 8-GPU baseboard)
    max_units: 8
    note: two NVSwitch ASICs; nine NVLinks from each GPU, each connected to an NVSwitch
market:
  observed_at: '2026-06-15'
  source: snapshot
key_features:
- HGX B100 8-GPU baseboard with two fourth-generation NVSwitch ASICs
- Nine NVLinks from each GPU to the NVSwitches
image: /images/gpus/nvidia-b100.jpg
tags:
- nvidia
- datacenter
- blackwell
updated: '2026-11-22'
sources:
- url: https://nvidianews.nvidia.com/news/aws-nvidia-generative-ai-innovation
  title: AWS and NVIDIA Extend Collaboration to Advance Generative AI Innovation (NVIDIA Newsroom, March 18, 2024)
  trust: 0.95
- url: https://docs.nvidia.com/hgx-platforms/fabric-manager-user-guide/index.html
  title: NVIDIA Fabric Manager User Guide (NVIDIA)
  trust: 0.95
---

## Overview

NVIDIA named the B100 Tensor Core GPU as part of its Blackwell platform on March 18, 2024, and documents an HGX B100 8-GPU baseboard with fourth-generation NVSwitches. NVIDIA publishes no specification page for the B100.
