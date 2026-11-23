---
id: guide/common-mistakes
type: guide
slug: common-mistakes
schema_version: 3.0
title: Mistakes to avoid
page_section: background
order: 8
mistakes:
- mistake: Buying on TFLOPS alone
  why: TFLOPS is peak compute, but NVIDIA notes that LLM token generation is memory-bound. A GPU with fewer TFLOPS and more memory bandwidth can generate tokens faster.
- mistake: Two consumer GPUs instead of one larger GPU
  why: NVIDIA lists no NVLink on the GeForce RTX 4090 and RTX 5090, so two cards talk over PCIe. On the H100, NVIDIA lists 900 GB/s for NVLink and 128 GB/s for PCIe Gen5. You get twice the VRAM, with a slower link between the cards.
- mistake: Ignoring quantization
  why: A 4-bit model's weights need a quarter of their 16-bit memory (0.5 bytes against 2 bytes per parameter), so a smaller card can often hold it.
- mistake: Buying a GPU for training when renting is cheaper
  why: Whether owning pays off depends on your hours of use; try your own hours in the buy-vs-rent table.
- mistake: Overlooking Apple silicon for inference
  why: Apple's unified memory is shared by CPU and GPU. Apple states the M1 Ultra can be configured with 128 GB at 800 GB/s, against 32 GB on a GeForce RTX 5090.
tags:
- gpu-buying-guide
- common-mistakes
updated: '2026-11-21'
sources:
- url: https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/
  title: 'Mastering LLM Techniques: Inference Optimization (NVIDIA Technical Blog)'
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/
  title: NVIDIA GeForce RTX 4090
  trust: 0.95
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5090/
  title: NVIDIA GeForce RTX 5090
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU
  trust: 0.95
- url: https://www.apple.com/newsroom/2022/03/apple-unveils-m1-ultra-the-worlds-most-powerful-chip-for-a-personal-computer/
  title: Apple unveils M1 Ultra (Apple Newsroom)
  trust: 0.95
---


