---
id: framework-support/tensorflow
type: framework-support
slug: tensorflow
schema_version: 2.1
title: TensorFlow
framework: framework/tensorflow
checked: '2026-11-22'
platforms:
- platform: cuda
  supported: true
  min_compute_capability: 3.5
  note: Ubuntu and Windows WSL2; TensorFlow 2.10 was the last release with GPU support on native Windows
  source: https://www.tensorflow.org/install/pip
- platform: rocm
  supported: true
  note: AMD's ROCm compatibility matrix lists TensorFlow
  source: https://rocm.docs.amd.com/en/latest/compatibility/compatibility-matrix.html
- platform: apple-silicon
  supported: false
  note: TensorFlow states there is no official GPU support for macOS
  source: https://www.tensorflow.org/install/pip
- platform: google-tpu
  supported: true
  source: https://www.tensorflow.org/guide/tpu
tags:
- tensorflow
- framework-support
updated: '2026-11-22'
sources:
- url: https://www.tensorflow.org/install/pip
  title: Install TensorFlow with pip (TensorFlow)
  trust: 0.95
- url: https://www.tensorflow.org/guide/tpu
  title: Use TPUs (TensorFlow guide)
  trust: 0.95
- url: https://rocm.docs.amd.com/en/latest/compatibility/compatibility-matrix.html
  title: ROCm compatibility matrix (AMD)
  trust: 0.9
---
