---
id: guide/common-mistakes
type: guide
slug: common-mistakes
schema_version: 1.1
title: Common Mistakes to Avoid
order: 7
mistakes:
- mistake: Buying based on TFLOPS alone
  why: TFLOPS measures peak compute, but LLM inference is memory-bandwidth-bound. A GPU with lower TFLOPS but higher memory bandwidth can be faster for inference.
- mistake: Getting 2× consumer GPUs instead of 1× larger GPU
  why: PCIe bandwidth between consumer GPUs is 50-100× slower than NVLink. You get 2× VRAM but communication overhead kills performance for training. For inference with tensor parallelism, it can work but with significant overhead.
- mistake: Ignoring quantization options
  why: A $1,600 RTX 4090 running a 4-bit quantized 70B model often beats a $30,000 H100 running the same model at FP16 for single-user inference. Quantization changes the cost equation dramatically.
- mistake: Buying a GPU for training when cloud is cheaper
  why: If you train for <100 hours/month, cloud is almost always cheaper. You only break even on purchased hardware at high utilization (>50%).
- mistake: Overlooking Apple Silicon for inference
  why: M4 Max (128GB) costs $3,500 and runs 70B models at 4-bit with decent speed. Silent, low power, no driver issues. For personal inference, it's often the best value.
- mistake: Not considering resale value
  why: NVIDIA datacenter GPUs depreciate 30-50% per generation. A $10K A100 is worth ~$4K now that H100 exists. Consumer GPUs hold value better.
tags:
- gpu-buying-guide
- common-mistakes
updated: '2026-11-19'
sources: []
---


