---
id: framework-support/onnx-runtime
type: framework-support
slug: onnx-runtime
schema_version: 2.1
title: ONNX Runtime
framework: framework/onnx-runtime
checked: '2026-11-22'
platforms:
- platform: cuda
  supported: true
  note: NVIDIA CUDA and NVIDIA TensorRT execution providers
  source: https://onnxruntime.ai/docs/execution-providers/
- platform: rocm
  supported: true
  note: AMD MIGraphX execution provider; the AMD ROCm execution provider is marked deprecated
  source: https://onnxruntime.ai/docs/execution-providers/
- platform: intel-gpu
  supported: true
  note: Intel OpenVINO execution provider
  source: https://onnxruntime.ai/docs/execution-providers/
- platform: apple-silicon
  supported: true
  note: CoreML execution provider, marked preview
  source: https://onnxruntime.ai/docs/execution-providers/
tags:
- onnx-runtime
- framework-support
updated: '2026-11-22'
sources:
- url: https://onnxruntime.ai/docs/execution-providers/
  title: Execution Providers (ONNX Runtime documentation)
  trust: 0.95
---
