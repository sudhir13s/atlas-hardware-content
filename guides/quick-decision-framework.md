---
id: guide/quick-decision-framework
type: guide
slug: quick-decision-framework
schema_version: 1.2
title: Quick decision
page_section: quick-decision
order: 1
decisions:
- scenario: Learning or experimenting
  recommendation: A free cloud tier (Colab, Kaggle) or the GPU you already have.
- scenario: Running LLMs locally for personal use
  recommendation: A consumer GPU with the most VRAM you can get, or a Mac with large unified memory and MLX.
  section: model-memory
- scenario: Fine-tuning 7B to 13B models
  recommendation: A 24 GB consumer GPU with QLoRA, or a rented datacenter GPU for a full fine-tune.
  section: model-memory
- scenario: Needing more than 80 GB in one GPU
  recommendation: A datacenter GPU (H100, A100, MI300X) or several GPUs.
  section: by-use-case
- scenario: Training from scratch under 70B parameters
  recommendation: Rent an H100 or A100 cluster; do not buy.
  section: buy-vs-rent
- scenario: Production inference at low volume
  recommendation: Serverless cloud (Modal, Replicate, Together), paying per token.
- scenario: Production inference at high volume
  recommendation: Dedicated cloud GPUs or co-located servers.
  section: buy-vs-rent
- scenario: Frontier training above 70B parameters
  recommendation: A multi-node datacenter cluster, through cloud or partnership only.
tags:
- gpu-buying-guide
- quick-decision-framework
updated: '2026-11-21'
sources: []
---
