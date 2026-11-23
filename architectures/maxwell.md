---
id: gpu-architecture/maxwell
type: gpu-architecture
slug: maxwell
schema_version: 3.0
title: NVIDIA Maxwell
name: Maxwell
vendor: NVIDIA
codename: GM107 / GM204 / GM200
year: 2014
predecessors:
- gpu-architecture/kepler
process_node: TSMC 28nm
segment: consumer + datacenter
representative_gpus: []
key_innovation: A redesigned multiprocessor (SMM) that NVIDIA states gives twice the energy efficiency of Kepler, on the same 28 nm process.
innovations:
- SMM multiprocessor in four 32-core processing blocks
- Much larger L2 cache (2048 KB on GM204 versus 512 KB on GK104)
- Dedicated shared memory per SM
- Efficiency gain without a node shrink
precision_support:
- FP64
- FP32
memory_tech: GDDR5
interconnect: PCI Express 3.0
tags:
- nvidia
- maxwell
- cuda
- efficiency
updated: '2026-11-21'
sources:
- url: https://developer.nvidia.com/blog/5-things-you-should-know-about-new-maxwell-gpu-architecture/
  title: 5 Things You Should Know About the New Maxwell GPU Architecture (NVIDIA Technical Blog, February 2014)
  trust: 0.95
- url: https://developer.nvidia.com/blog/maxwell-most-advanced-cuda-gpu-ever-made
  title: 'Maxwell: The Most Advanced CUDA GPU Ever Made (NVIDIA Technical Blog, September 2014)'
  trust: 0.95
- url: https://developer.nvidia.com/maxwell-compute-architecture
  title: NVIDIA Maxwell Compute Architecture
  trust: 0.95
- url: https://docs.nvidia.com/cuda/maxwell-tuning-guide/
  title: NVIDIA Maxwell Tuning Guide
  trust: 0.95
- url: https://www.nvidia.com/content/geforce-gtx/gtx_980_user_guide.pdf
  title: NVIDIA GeForce GTX 980 Installation Guide
  trust: 0.95
- url: https://developer.nvidia.com/blog/accelerating-hyperscale-datacenter-applications-tesla-gpus/
  title: Accelerating Hyperscale Data Center Applications with NVIDIA M40 and M4 GPUs (NVIDIA Technical Blog)
  trust: 0.95
- url: https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/documents/NVIDIA-Kepler-GK110-GK210-Architecture-Whitepaper.pdf
  title: NVIDIA Kepler GK110/GK210 Architecture Whitepaper
  trust: 0.95
---

## What Changed

Maxwell stayed on the **same 28 nm process** as Kepler, so its gains came from design. NVIDIA put
the energy efficiency of the first Maxwell GPU (GM107, GeForce GTX 750 Ti, 2014) at nearly twice
that of Kepler.

- **SMM** splits each multiprocessor into four 32-core processing blocks, each with its own warp
  scheduler.
- **L2 cache** grew to 2048 KB on GM107 (256 KB on GK107) and on GM204 (512 KB on GK104).
- **Shared memory** became a dedicated block per SM, separate from the L1 cache.

The second generation (GM204, GeForce GTX 980 and 970) followed in September 2014. The datacenter
**Tesla M40** (GM200) carries 12 GB of GDDR5. NVIDIA states that Maxwell runs double precision at
1/32 of its single-precision rate.
