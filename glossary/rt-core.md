---
id: glossary-term/rt-core
type: glossary-term
slug: rt-core
schema_version: 1.0
title: "RT Core"
term: "RT Core"
category: compute
examples: ["1st-gen RT Cores on Turing", "3rd-gen RT Cores on Ada Lovelace", "AMD Ray Accelerators; Intel RT units"]
related: [glossary-term/cuda-core, glossary-term/tensor-core]
tags: [compute, rt-core, ray-tracing]
updated: 2026-07-17
sources:
  - { url: "https://www.nvidia.com/en-us/technologies/rtx/", title: "NVIDIA RTX Ray Tracing", trust: 0.9 }
---

## Definition
An RT Core is a fixed-function unit that accelerates ray tracing — specifically bounding-volume-hierarchy
traversal and ray-triangle intersection — the geometry math behind realistic lighting, reflections, and
shadows. AMD's equivalent is the Ray Accelerator; Intel has dedicated ray-tracing units.

## Why You Care
RT Cores are a graphics feature, not an AI one — included here because they are the third specialized
engine (with CUDA cores and Tensor Cores) that a modern GPU spends die area on, and understanding the
split clarifies why "AI performance" and "gaming performance" are different numbers. For pure AI
workloads, RT Core count is irrelevant; for a workstation doing both rendering and ML, it is not.
