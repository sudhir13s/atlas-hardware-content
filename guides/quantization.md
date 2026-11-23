---
id: guide/quantization
type: guide
slug: quantization
schema_version: 3.0
title: 'Quantization: run bigger models on smaller GPUs'
page_section: background
order: 6
table:
  columns:
  - Method
  - Bits
  - Memory savings
  - Quality
  - Best for
  rows:
  - - FP16 and BF16
    - '16'
    - Baseline
    - Full
    - Training, fine-tuning
  - - INT8 (LLM.int8() in bitsandbytes)
    - '8'
    - 50% of weights
    - No degradation up to 175B parameters (its paper)
    - Inference
  - - GPTQ
    - 3 or 4
    - 75% of weights at 4 bits
    - Negligible accuracy loss at 3 or 4 bits (its paper)
    - GPU inference (vLLM)
  - - AWQ
    - '4'
    - 75% of weights
    - Activation-aware, weight-only
    - GPU inference (vLLM)
  - - GGUF (llama.cpp)
    - 1.5 to 8
    - About 50% to 90% of weights
    - Varies with the quant level
    - CPU, Apple silicon (Metal), NVIDIA (CUDA), AMD (HIP)
tags:
- gpu-buying-guide
- quantization
updated: '2026-11-21'
sources:
- url: https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/
  title: 'Mastering LLM Techniques: Inference Optimization (NVIDIA Technical Blog)'
  trust: 0.95
- url: https://arxiv.org/abs/2208.07339
  title: 'LLM.int8(): 8-bit Matrix Multiplication for Transformers at Scale'
  trust: 0.95
- url: https://arxiv.org/abs/2210.17323
  title: 'GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers'
  trust: 0.95
- url: https://arxiv.org/abs/2306.00978
  title: 'AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration'
  trust: 0.95
- url: https://github.com/ggml-org/llama.cpp
  title: llama.cpp
  trust: 0.9
- url: https://docs.vllm.ai/en/latest/features/quantization/
  title: Quantization - vLLM documentation
  trust: 0.9
---

## Overview

Quantization stores weights at 8 or 4 bits instead of 16. **Weight memory** is bits ÷ 8 bytes per parameter: 2 at 16-bit (NVIDIA: 7B × 2 bytes ≈ 14 GB), 1 at 8-bit, 0.5 at 4-bit. Savings shown are for weights only, before quantization scales.

## Takeaway

For inference, start with a 4-bit method (GPTQ, AWQ or a 4-bit GGUF): weights take about a quarter of their 16-bit memory. Use 16-bit for training.
