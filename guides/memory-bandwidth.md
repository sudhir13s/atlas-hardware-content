---
id: guide/memory-bandwidth
type: guide
slug: memory-bandwidth
schema_version: 1.2
title: 'Memory bandwidth: why speed matters'
page_section: background
order: 4
points:
- name: HBM3e
  text: 4,800 to 8,000 GB/s. Best for large-scale inference and training.
- name: HBM3
  text: 2,000 to 5,300 GB/s. Strong for datacenter workloads.
- name: GDDR6X and GDDR7
  text: 1,000 to 1,800 GB/s. Good for local inference.
- name: Unified LPDDR5X
  text: 400 to 800 GB/s. Lower bandwidth, but no copy between CPU and GPU memory.
tags:
- gpu-buying-guide
- memory-bandwidth
updated: '2026-11-21'
sources: []
---

## Overview

LLM inference is limited by memory bandwidth, not compute. The GPU spends most of its time reading model weights from memory, so higher bandwidth means faster token generation.

## Takeaway

Rule: tokens per second is at most bandwidth divided by the bytes read per token. A 7B model at 16-bit reads 14 GB per token, so 3,350 GB/s of bandwidth allows about 240 tokens per second.
