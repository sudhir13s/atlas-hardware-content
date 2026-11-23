---
id: guide/software-ecosystem
type: guide
slug: software-ecosystem
schema_version: 3.0
title: 'Software ecosystem: CUDA, ROCm and MLX'
page_section: background
order: 5
points:
- name: NVIDIA CUDA
  text: NVIDIA's development environment for GPU-accelerated applications on its GPUs. vLLM lists NVIDIA CUDA as a supported GPU platform.
- name: AMD ROCm
  text: AMD's open-source GPU computing platform for AMD Instinct, Radeon and Ryzen AI devices, on Linux and Windows. vLLM lists AMD ROCm as a supported GPU platform.
- name: Apple MLX
  text: An array framework for Apple silicon from Apple machine learning research. Arrays live in shared memory, so CPU and GPU operations need no data copy.
tags:
- gpu-buying-guide
- software-ecosystem
updated: '2026-11-21'
sources:
- url: https://developer.nvidia.com/cuda-toolkit
  title: CUDA Toolkit (NVIDIA Developer)
  trust: 0.95
- url: https://rocm.docs.amd.com/en/latest/
  title: AMD ROCm documentation
  trust: 0.95
- url: https://github.com/ml-explore/mlx
  title: 'MLX: an array framework for Apple silicon'
  trust: 0.95
- url: https://docs.vllm.ai/en/latest/getting_started/installation/
  title: Installation - vLLM documentation
  trust: 0.9
---

## Overview

The software stack decides which frameworks and tools run on a GPU.
