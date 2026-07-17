---
id: glossary-term/mig
type: glossary-term
slug: mig
schema_version: 1.0
title: "MIG (Multi-Instance GPU)"
term: "MIG (Multi-Instance GPU)"
category: compute
examples: ["Up to 7 isolated instances on an A100", "MIG on H100 with per-instance memory and cache"]
related: []
tags: [compute, mig, virtualization]
updated: 2026-07-17
sources:
  - { url: "https://www.nvidia.com/en-us/technologies/multi-instance-gpu/", title: "NVIDIA Multi-Instance GPU", trust: 0.9 }
---

## Definition
MIG partitions a single physical GPU (Ampere onward, on A100/H100-class parts) into up to seven fully
isolated instances, each with its own slice of compute, memory, and cache. Instances are hardware-isolated
so one tenant's work cannot interfere with another's.

## Why You Care
Many inference and development jobs cannot use a whole 80 GB accelerator, so running them on a full GPU
wastes expensive silicon. MIG lets one card serve several independent workloads at guaranteed quality of
service — valuable for cloud multi-tenancy and for right-sizing inference. If your workloads are small,
MIG support can multiply the effective capacity of each GPU you buy.
