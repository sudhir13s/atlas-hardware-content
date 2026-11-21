---
id: glossary-term/mig
type: glossary-term
slug: mig
schema_version: 1.0
title: "MIG (Multi-Instance GPU)"
term: "MIG (Multi-Instance GPU)"
category: compute
examples: ["Up to 7 GPU instances on an A100", "Up to 7 MIGs at 10 GB each on H100 SXM"]
related: []
tags: [compute, mig, virtualization]
updated: '2026-11-21'
sources:
  - { url: "https://www.nvidia.com/en-us/technologies/multi-instance-gpu/", title: "NVIDIA Multi-Instance GPU (NVIDIA)", trust: 0.95 }
  - { url: "https://developer.nvidia.com/blog/nvidia-ampere-architecture-in-depth/", title: "NVIDIA Ampere Architecture In-Depth (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/h100/", title: "NVIDIA H100 Tensor Core GPU (NVIDIA)", trust: 0.95 }
  - { url: "https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/", title: "NVIDIA Hopper Architecture In-Depth (NVIDIA)", trust: 0.95 }
---

## Definition
MIG partitions one supported NVIDIA GPU into as many as seven instances, each isolated with its own
high-bandwidth memory, cache and compute cores. The A100 (Ampere) supports it, and NVIDIA lists
Hopper, Blackwell and Rubin GPUs as supporting it.

## Why You Care
NVIDIA states that MIG gives each instance guaranteed quality of service, and that a failure in one
instance does not affect applications in the others. A job too small for a whole GPU can run on one
instance while other jobs use the rest.
