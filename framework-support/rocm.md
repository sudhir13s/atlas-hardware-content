---
id: framework-support/rocm
type: framework-support
slug: rocm
schema_version: 2.0
title: ROCm
checked: '2026-11-22'
platforms:
- platform: rocm
  supported: true
  note: AMD's list of supported GPUs on Linux; the Radeon RX 7900 XTX only on the Ubuntu and RHEL releases AMD lists
  gpus:
  - gpu/amd-mi100
  - gpu/amd-mi210
  - gpu/amd-mi250x
  - gpu/amd-mi300x
  - gpu/amd-mi325x
  - gpu/amd-rx-7900-xtx
  source: https://rocm.docs.amd.com/projects/install-on-linux/en/latest/reference/system-requirements.html
tags:
- rocm
- framework-support
updated: '2026-11-22'
sources:
- url: https://rocm.docs.amd.com/projects/install-on-linux/en/latest/reference/system-requirements.html
  title: System requirements (Linux), supported GPUs (AMD ROCm documentation)
  trust: 0.95
---
