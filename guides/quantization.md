---
id: guide/quantization
type: guide
slug: quantization
schema_version: 1.1
title: 'Quantization: Run Bigger Models on Smaller GPUs'
order: 4
quantization_methods:
- method: FP16/BF16
  bits: '16'
  memory_savings: Baseline
  quality: Full
  best_for: Training, fine-tuning
- method: INT8 (bitsandbytes)
  bits: '8'
  memory_savings: ~50%
  quality: Near-lossless
  best_for: Inference, QLoRA training
- method: GPTQ
  bits: '4'
  memory_savings: ~75%
  quality: Good (calibrated)
  best_for: GPU inference (exl2, vLLM)
- method: AWQ
  bits: '4'
  memory_savings: ~75%
  quality: Good (activation-aware)
  best_for: GPU inference (vLLM)
- method: GGUF (llama.cpp)
  bits: 2-8
  memory_savings: 50-85%
  quality: Varies by quant level
  best_for: CPU/Metal/CUDA (flexible)
tags:
- gpu-buying-guide
- quantization
updated: '2026-11-19'
sources: []
---

## Overview

Quantization reduces model precision from FP16 (16 bits) to INT8 (8 bits) or INT4 (4 bits), cutting memory by 2-4×. Quality loss is minimal for inference.

## Takeaway

Recommendation: for inference, start with Q4_K_M (GGUF) or AWQ — good quality at 4× memory savings. Use FP16 for training and fine-tuning.
