---
id: gpu-architecture/<slug>
type: gpu-architecture
slug: <slug>
schema_version: 3.0              # the schema's current version; the schema refuses any other
title: "<Human Readable Name>"
name: "<Architecture Name>"
vendor: NVIDIA                     # NVIDIA | AMD | Intel
codename: "<internal codename>"    # optional
year: <YYYY>
predecessors: [gpu-architecture/<slug>]   # optional; FKs, the direct line first. What follows is never stored here
process_node: "<e.g. TSMC 4N>"
segment: "<consumer | datacenter | consumer + datacenter>"
representative_gpus: [gpu/<slug>]         # FKs
key_innovation: "<the one thing this generation introduced>"
innovations: ["<innovation>", "<innovation>"]
precision_support: ["FP32", "FP16", "..."]
memory_tech: "<e.g. GDDR6X, HBM3>"
interconnect: "<e.g. PCIe 4.0, NVLink 3.0>"
tags: [<tag>]
updated: <YYYY-MM-DD>
sources:
  - { url: "<url>", title: "<title>", trust: 0.9 }
---

## What Changed
<What this generation changed relative to its predecessor, and why it matters for AI workloads.>
