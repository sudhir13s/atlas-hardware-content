---
id: framework-support/deepspeed
type: framework-support
slug: deepspeed
schema_version: 2.0
title: DeepSpeed
checked: '2026-11-22'
platforms:
- platform: cuda
  supported: true
  note: the README names Pascal, Volta, Ampere and Hopper GPUs
  gpus:
  - gpu/nvidia-v100-16gb
  - gpu/nvidia-v100-32gb
  - gpu/nvidia-a100-40gb
  - gpu/nvidia-a100-80gb
  - gpu/nvidia-a4000
  - gpu/nvidia-a5000
  - gpu/nvidia-a6000
  - gpu/nvidia-rtx-3080
  - gpu/nvidia-rtx-3090
  - gpu/nvidia-h100-pcie
  - gpu/nvidia-h100-sxm
  - gpu/nvidia-h200
  source: https://github.com/deepspeedai/DeepSpeed
- platform: rocm
  supported: true
  note: the README names MI100 and MI200
  gpus:
  - gpu/amd-mi100
  - gpu/amd-mi210
  - gpu/amd-mi250x
  source: https://github.com/deepspeedai/DeepSpeed
- platform: intel-gaudi
  supported: true
  note: Gaudi 2, validated by Intel and upstream
  gpus:
  - gpu/intel-gaudi-2
  source: https://github.com/deepspeedai/DeepSpeed
- platform: intel-gpu
  supported: true
  note: Data Center GPU Max series, validated by Intel and upstream
  gpus:
  - gpu/intel-dc-gpu-max-1550
  source: https://github.com/deepspeedai/DeepSpeed
tags:
- deepspeed
- framework-support
updated: '2026-11-22'
sources:
- url: https://github.com/deepspeedai/DeepSpeed
  title: DeepSpeed repository README, requirements and contributed hardware support (DeepSpeed)
  trust: 0.9
---
