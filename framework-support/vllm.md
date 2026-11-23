---
id: framework-support/vllm
type: framework-support
slug: vllm
schema_version: 3.0
title: vLLM
framework: framework/vllm
checked: '2026-11-22'
platforms:
- platform: cuda
  supported: true
  min_compute_capability: 7.5
  note: Linux; vLLM does not support Windows natively
  source: https://docs.vllm.ai/en/latest/getting_started/installation/gpu.html
- platform: rocm
  supported: true
  note: MI200s (gfx90a), MI300 (gfx942) and Radeon RX 7900 series (gfx1100/1101) among the listed GPUs
  gpus:
  - gpu/amd-mi210
  - gpu/amd-mi250x
  - gpu/amd-mi300x
  - gpu/amd-mi325x
  - gpu/amd-rx-7900-xtx
  source: https://docs.vllm.ai/en/latest/getting_started/installation/gpu.html
- platform: intel-gpu
  supported: true
  note: Intel Data Center GPU and Intel Arc GPU
  source: https://docs.vllm.ai/en/latest/getting_started/installation/gpu.html
- platform: apple-silicon
  supported: true
  note: through vLLM-Metal
  source: https://docs.vllm.ai/en/latest/getting_started/installation/
tags:
- vllm
- framework-support
updated: '2026-11-22'
sources:
- url: https://docs.vllm.ai/en/latest/getting_started/installation/gpu.html
  title: GPU installation (vLLM documentation)
  trust: 0.95
- url: https://docs.vllm.ai/en/latest/getting_started/installation/
  title: Installation (vLLM documentation)
  trust: 0.95
---


