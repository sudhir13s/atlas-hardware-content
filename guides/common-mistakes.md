---
id: guide/common-mistakes
type: guide
slug: common-mistakes
schema_version: 1.2
title: Mistakes to avoid
page_section: background
order: 8
mistakes:
- mistake: Buying on TFLOPS alone
  why: TFLOPS is peak compute, but LLM inference is limited by memory bandwidth. A GPU with fewer TFLOPS and more bandwidth can be faster for inference.
- mistake: Two consumer GPUs instead of one larger GPU
  why: PCIe between consumer cards is an order of magnitude or more slower than NVLink. You get twice the VRAM, but communication overhead hurts training. For inference with tensor parallelism it can work, with real overhead.
- mistake: Ignoring quantization
  why: A 4-bit model needs a quarter of the 16-bit memory, so a smaller, cheaper card can often run it for one user.
- mistake: Buying a GPU for training when renting is cheaper
  why: If you train only a few hours a month, renting almost always costs less. Owning pays off only at high use; try your own hours in the buy-vs-rent table.
- mistake: Overlooking Apple silicon for inference
  why: Large unified memory runs big quantized models quietly, at low power and with no driver setup. For personal inference it is often the simplest option.
- mistake: Ignoring resale value
  why: Datacenter GPUs lose value when the next generation ships; consumer cards usually hold value better. Check recent sold listings, not list prices.
tags:
- gpu-buying-guide
- common-mistakes
updated: '2026-11-21'
sources: []
---
