---
id: framework-support/jax
type: framework-support
slug: jax
schema_version: 3.0
title: JAX
framework: framework/jax
checked: '2026-11-22'
platforms:
- platform: cuda
  supported: true
  note: Linux; experimental on Windows WSL2, not supported on native Windows
  source: https://docs.jax.dev/en/latest/installation.html
- platform: rocm
  supported: true
  note: through a ROCm JAX plugin maintained by AMD; Linux x86_64, experimental on Windows WSL2
  source: https://docs.jax.dev/en/latest/installation.html
- platform: intel-gpu
  supported: true
  note: experimental, through Intel's oneAPI plugin; Linux x86_64
  source: https://docs.jax.dev/en/latest/installation.html
- platform: google-tpu
  supported: true
  note: Linux x86_64
  source: https://docs.jax.dev/en/latest/installation.html
tags:
- jax
- framework-support
updated: '2026-11-22'
sources:
- url: https://docs.jax.dev/en/latest/installation.html
  title: Installation (JAX documentation)
  trust: 0.95
---


