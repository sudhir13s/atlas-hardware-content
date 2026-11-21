---
id: guide/quantization
type: guide
slug: quantization
schema_version: 1.2
title: 'Quantization: run bigger models on smaller GPUs'
page_section: background
order: 6
table:
  columns: [Method, Bits, Memory savings, Quality, Best for]
  rows:
  - [FP16 and BF16, '16', Baseline, Full, 'Training, fine-tuning']
  - [INT8 (bitsandbytes), '8', About 50%, Near-lossless, 'Inference, QLoRA training']
  - [GPTQ, '4', About 75%, Good (calibrated), 'GPU inference (exl2, vLLM)']
  - [AWQ, '4', About 75%, Good (activation-aware), GPU inference (vLLM)]
  - [GGUF (llama.cpp), 2 to 8, 50% to 85%, Varies with the quant level, 'CPU, Metal and CUDA']
tags:
- gpu-buying-guide
- quantization
updated: '2026-11-21'
sources: []
---

## Overview

Quantization lowers model precision from 16-bit to 8-bit or 4-bit, cutting memory by 2 to 4 times. For inference the quality loss is usually small.

## Takeaway

For inference, start with Q4_K_M (GGUF) or AWQ: good quality at about a quarter of the memory. Use 16-bit for training and fine-tuning.
