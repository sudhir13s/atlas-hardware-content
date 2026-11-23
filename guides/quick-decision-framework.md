---
id: guide/quick-decision-framework
type: guide
slug: quick-decision-framework
schema_version: 3.0
title: Quick decision
page_section: quick-decision
order: 1
decisions:
- scenario: Learning or experimenting
  recommendation: A free cloud notebook (Colab and Kaggle both state free GPU access, with limits) or the GPU you already have.
- scenario: Running LLMs locally for personal use
  recommendation: A consumer GPU with the most VRAM you can get, or a Mac with large unified memory and MLX.
  section: model-memory
- scenario: Fine-tuning 7B to 13B models
  recommendation: A single GPU with QLoRA (its authors fine-tuned a 65B model on one 48 GB GPU), or a rented datacenter GPU for a full fine-tune.
  section: model-memory
- scenario: Needing more than 80 GB in one GPU
  recommendation: A datacenter GPU with more memory (NVIDIA H200 141 GB, AMD Instinct MI300X 192 GB, AMD Instinct MI325X 256 GB) or several GPUs.
  section: by-use-case
- scenario: Training a model from scratch
  recommendation: Compare renting a GPU cluster with buying before you commit.
  section: buy-vs-rent
- scenario: Production inference at low volume
  recommendation: 'Serverless cloud (Modal, Replicate, Together), paying for use: per second of GPU time or per token, depending on the service.'
- scenario: Production inference at high volume
  recommendation: Dedicated cloud GPUs or co-located servers.
  section: buy-vs-rent
- scenario: Training at frontier scale
  recommendation: A multi-node datacenter cluster.
tags:
- gpu-buying-guide
- quick-decision-framework
updated: '2026-11-21'
sources:
- url: https://research.google.com/colaboratory/faq.html
  title: Google Colab FAQ
  trust: 0.95
- url: https://www.kaggle.com/docs/efficient-gpu-usage
  title: Efficient GPU Usage Tips (Kaggle documentation)
  trust: 0.95
- url: https://github.com/ml-explore/mlx
  title: 'MLX: an array framework for Apple silicon'
  trust: 0.95
- url: https://arxiv.org/abs/2305.14314
  title: 'QLoRA: Efficient Finetuning of Quantized LLMs'
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h200/
  title: NVIDIA H200 Tensor Core GPU
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html
  title: AMD Instinct MI300X Accelerators
  trust: 0.95
- url: https://www.amd.com/en/products/accelerators/instinct/mi300/mi325x.html
  title: AMD Instinct MI325X Accelerators
  trust: 0.95
- url: https://modal.com/pricing
  title: Modal pricing
  trust: 0.9
- url: https://replicate.com/pricing
  title: Replicate pricing
  trust: 0.9
- url: https://www.together.ai/pricing
  title: Together AI pricing
  trust: 0.9
---


