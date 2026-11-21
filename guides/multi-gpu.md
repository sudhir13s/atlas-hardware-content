---
id: guide/multi-gpu
type: guide
slug: multi-gpu
schema_version: 1.2
title: 'Multi-GPU: when one card is not enough'
page_section: background
order: 7
points:
- name: NVLink
  text: A high-bandwidth GPU-to-GPU link (600 to 900 GB/s) that tensor parallelism needs. It is found on datacenter GPUs; consumer GPUs do not have it.
- name: PCIe
  text: 'The standard connection (32 to 64 GB/s). It works for pipeline parallelism but is too slow for tensor parallelism: two cards over PCIe give twice the VRAM, not twice the speed.'
- name: Apple UltraFusion
  text: A die-to-die link in the Ultra chips of Apple's M-series. The two dies act as one GPU, with no software setup.
tags:
- gpu-buying-guide
- multi-gpu
updated: '2026-11-21'
sources: []
---

## Overview

Several cards add memory, but only a fast link lets them add speed.

## Takeaway

Rule: for multi-GPU training, plan on NVLink-capable datacenter GPUs or rent them. Several consumer cards are a compromise.
