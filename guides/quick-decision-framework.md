---
id: guide/quick-decision-framework
type: guide
slug: quick-decision-framework
schema_version: 1.1
title: Quick Decision Framework
order: 8
decisions:
- scenario: Learning / experimenting
  recommendation: Free cloud tier (Colab, Kaggle) or your existing GPU
  icon: 🟢
- scenario: Running LLMs locally for personal use
  recommendation: RTX 4090/5090 ($1.6-2K) or Mac M4 Max ($2.5-3.5K)
  icon: 🟢
- scenario: Fine-tuning 7-13B models
  recommendation: RTX 4090 (24GB) with QLoRA, or cloud A100 for full fine-tune
  icon: 🟡
- scenario: Training from scratch (<70B)
  recommendation: Cloud H100/A100 cluster — rent, don't buy
  icon: 🔵
- scenario: Production inference (low volume)
  recommendation: Serverless cloud (Modal, Replicate, Together) — pay per token
  icon: 🔵
- scenario: Production inference (high volume)
  recommendation: Dedicated cloud GPUs or co-located servers with H100/L40S
  icon: 🟣
- scenario: Frontier model training (70B+)
  recommendation: Multi-node H100/B200 cluster — cloud or partnership only
  icon: 🔴
decision_flowchart:
- question: Need >80GB VRAM?
  answer: Datacenter GPU (H100, A100, MI300X)
- question: Budget <$2K?
  answer: RTX 4090 or RTX 5090
- question: Mac user?
  answer: M4 Max/Ultra with MLX
- question: Just experimenting?
  answer: Cloud (free tier first)
- question: Production serving?
  answer: Cloud serverless (Modal, Replicate)
tags:
- gpu-buying-guide
- quick-decision-framework
updated: '2026-11-19'
sources: []
---


