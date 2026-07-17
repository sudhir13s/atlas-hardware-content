---
id: glossary-term/nvlink
type: glossary-term
slug: nvlink
schema_version: 1.0
title: "NVLink"
term: "NVLink"
category: interconnect
examples: ["NVLink 1.0 on Tesla P100", "NVLink 4.0 on H100", "NVLink 5.0 on Blackwell (GB200 NVL72)"]
related: [glossary-term/nvswitch, glossary-term/pcie]
tags: [interconnect, nvlink, scale-out]
updated: 2026-07-17
sources:
  - { url: "https://www.nvidia.com/en-us/data-center/nvlink/", title: "NVIDIA NVLink", trust: 0.9 }
---

## Definition
NVLink is NVIDIA's proprietary high-bandwidth, low-latency interconnect for connecting GPUs directly to
each other (and to Grace CPUs), bypassing the slower PCIe bus. Each generation has raised per-GPU
bandwidth substantially, reaching well over 1 TB/s aggregate on recent parts.

## Why You Care
Training a model too large for one GPU means splitting it across many, and those GPUs must exchange
gradients and activations constantly. NVLink makes that exchange fast enough that dozens of GPUs behave
like one large accelerator. Its absence on consumer cards (Ada, Blackwell GeForce) is a deliberate
market segmentation: it keeps cheap cards from being cheaply clustered for training.
