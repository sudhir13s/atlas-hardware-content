---
id: glossary-term/vram
type: glossary-term
slug: vram
schema_version: 1.0
title: "VRAM (Video Memory)"
term: "VRAM (Video Memory)"
category: memory
examples: ["24 GB VRAM on RTX 4090", "80 GB on H100 SXM", "192 GB on MI300X"]
related: [glossary-term/hbm, glossary-term/gddr6, glossary-term/memory-bandwidth]
tags: [memory, vram, capacity]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Video_random-access_memory", title: "Video RAM — Wikipedia", trust: 0.8 }
---

## Definition
VRAM is the memory physically attached to the GPU (HBM on datacenter cards, GDDR on consumer cards) that
holds everything the GPU is actively working on — for AI, the model weights, activations, optimizer
state, and KV cache. It is separate from and much faster than system RAM.

## Why You Care
VRAM capacity is often the first thing that decides whether you can run a model at all: if the weights
plus working memory do not fit, the job fails or must be split across GPUs. A rough rule for inference is
that a model needs roughly (parameters × bytes-per-parameter) of VRAM — e.g. a 70B model in FP16 needs
~140 GB, which is why it does not fit on a single 24 GB consumer card without quantization.
