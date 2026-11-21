---
id: glossary-term/nvswitch
type: glossary-term
slug: nvswitch
schema_version: 1.0
title: "NVSwitch"
term: "NVSwitch"
category: interconnect
examples: ["NVL72: 72 GPUs in one NVLink domain (Blackwell)"]
related: [glossary-term/nvlink]
tags: [interconnect, nvswitch, fabric]
updated: '2026-11-21'
sources:
  - { url: "https://www.nvidia.com/en-us/data-center/nvlink/", title: "NVIDIA NVLink and NVLink Switch (NVIDIA)", trust: 0.95 }
  - { url: "https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/", title: "NVIDIA Blackwell Architecture (NVIDIA)", trust: 0.95 }
---

## Definition
NVSwitch, which NVIDIA's current pages call the NVLink Switch, is a switch chip that connects multiple
NVLinks to give all-to-all GPU communication. It also extends NVLink connections across nodes.

## Why You Care
Point-to-point NVLink alone couples only a few GPUs. With NVLink Switch chips, NVIDIA's NVL72 rack
places 72 GPUs in one NVLink domain, which NVIDIA states can be used as a single accelerator.
