---
id: guide/software-ecosystem
type: guide
slug: software-ecosystem
schema_version: 1.2
title: 'Software ecosystem: CUDA, ROCm and MLX'
page_section: background
order: 5
points:
- name: NVIDIA CUDA
  text: The most mature stack. PyTorch, TensorFlow, JAX, TensorRT, vLLM and DeepSpeed all assume CUDA first. For the least friction, choose NVIDIA.
- name: AMD ROCm
  text: Catching up fast. PyTorch works well; TensorFlow and JAX have gaps, and vLLM and DeepSpeed support keeps improving. Expect the occasional compatibility issue.
- name: Apple MLX
  text: 'Excellent for local inference on a Mac: light, fast and Apple-optimized. It has no multi-GPU support and limited training support, and many libraries are CUDA-only. Best for personal use.'
tags:
- gpu-buying-guide
- software-ecosystem
updated: '2026-11-21'
sources: []
---

## Overview

The software stack decides how much friction you meet before the first token.
