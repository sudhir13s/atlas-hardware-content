---
id: framework-support/pytorch
type: framework-support
slug: pytorch
schema_version: 2.1
title: PyTorch
framework: framework/pytorch
checked: '2026-11-22'
platforms:
- platform: cuda
  supported: true
  source: https://docs.pytorch.org/docs/2.15/notes/cuda.html
- platform: rocm
  supported: true
  note: PyTorch for HIP reuses the torch.cuda interfaces
  source: https://docs.pytorch.org/docs/2.15/notes/hip.html
- platform: apple-silicon
  supported: true
  note: the mps device, on macOS with Metal
  source: https://docs.pytorch.org/docs/2.15/notes/mps.html
- platform: intel-gpu
  supported: true
  note: the xpu device; Data Center GPU Max on Linux, Arc A-Series on Windows 11 and Ubuntu
  gpus:
  - gpu/intel-dc-gpu-max-1550
  - gpu/intel-arc-a770
  source: https://docs.pytorch.org/docs/2.15/notes/get_start_xpu.html
- platform: intel-gaudi
  supported: true
  note: Intel states its Gaudi software is integrated with PyTorch
  source: https://docs.habana.ai/en/latest/PyTorch/index.html
tags:
- pytorch
- framework-support
updated: '2026-11-22'
sources:
- url: https://docs.pytorch.org/docs/2.15/notes/cuda.html
  title: CUDA semantics (PyTorch 2.15 documentation)
  trust: 0.95
- url: https://docs.pytorch.org/docs/2.15/notes/hip.html
  title: HIP (ROCm) semantics (PyTorch 2.15 documentation)
  trust: 0.95
- url: https://docs.pytorch.org/docs/2.15/notes/mps.html
  title: MPS backend (PyTorch 2.15 documentation)
  trust: 0.95
- url: https://docs.pytorch.org/docs/2.15/notes/get_start_xpu.html
  title: Getting Started on Intel GPU (PyTorch 2.15 documentation)
  trust: 0.95
- url: https://docs.habana.ai/en/latest/PyTorch/index.html
  title: PyTorch (Intel Gaudi documentation)
  trust: 0.9
---
