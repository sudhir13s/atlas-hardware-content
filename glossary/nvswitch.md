---
id: glossary-term/nvswitch
type: glossary-term
slug: nvswitch
schema_version: 1.0
title: "NVSwitch"
term: "NVSwitch"
category: interconnect
examples: ["8-GPU all-to-all in a DGX/HGX server", "GB200 NVL72 rack: 72 GPUs in one NVLink domain"]
related: [glossary-term/nvlink]
tags: [interconnect, nvswitch, fabric]
updated: 2026-07-17
sources:
  - { url: "https://www.nvidia.com/en-us/data-center/nvlink/", title: "NVIDIA NVLink and NVSwitch", trust: 0.9 }
---

## Definition
NVSwitch is a switch chip that connects many NVLink-capable GPUs in an all-to-all topology, so every GPU
can talk to every other at full NVLink bandwidth rather than only its immediate neighbors. It is the
fabric that turns a tray or rack of GPUs into a single NVLink domain.

## Why You Care
Point-to-point NVLink alone limits how many GPUs can be tightly coupled. NVSwitch is what lets an 8-GPU
HGX baseboard — or a 72-GPU GB200 NVL72 rack — act as one memory-coherent accelerator, which is the unit
frontier models are actually trained on. When you see "NVL72" or "all-to-all bandwidth," NVSwitch is the
enabling hardware.
