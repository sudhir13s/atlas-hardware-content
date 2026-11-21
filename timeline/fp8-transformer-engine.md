---
id: timeline-event/fp8-transformer-engine
type: timeline-event
slug: fp8-transformer-engine
schema_version: 1.0
title: "FP8 and the Transformer Engine arrive with Hopper"
date: 2022-03-22
vendor: NVIDIA
event_type: milestone
architecture_id: gpu-architecture/hopper
tags: [nvidia, hopper, fp8, transformer-engine, milestone]
updated: '2026-11-21'
sources:
  - { url: "https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/", title: "NVIDIA Hopper Architecture In-Depth (NVIDIA Technical Blog)", trust: 0.95 }
  - { url: "https://nvidianews.nvidia.com/news/nvidia-announces-hopper-architecture-the-next-generation-of-accelerated-computing", title: "NVIDIA Announces Hopper Architecture (NVIDIA Newsroom, 22 Mar 2022)", trust: 0.95 }
---

## Description
Hopper, announced on 22 March 2022, added 8-bit floating point (FP8) in two formats, E4M3 and E5M2. Its
Transformer Engine analyses Tensor Core output statistics to choose between FP8 and 16-bit math per
layer and rescales values to fit. NVIDIA states that FP8 halves storage and doubles throughput compared
with FP16 or BF16.
