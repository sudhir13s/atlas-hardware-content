---
id: name-decoder/nvidia
type: name-decoder
slug: nvidia
schema_version: 3.0
title: NVIDIA product-name decoder
vendor: NVIDIA
prefixes:
- symbol: RTX
  meaning: GeForce RTX 20, 30, 40 and 50 Series consumer cards; NVIDIA introduced the RTX 20 Series with RT Cores and Tensor Cores
- symbol: GTX
  meaning: Earlier GeForce prefix, for example the GeForce GTX 1080 Ti (2017)
- symbol: A / H / B / L
  meaning: 'Data center GPUs: A100 is NVIDIA Ampere, H100 is Hopper and B200 is Blackwell (the letter matches the architecture''s initial); the L40S is Ada Lovelace'
numbering: 'GeForce RTX: the leading digits name the series, and NVIDIA''s comparison page gives one architecture per series (20 = Turing, 30 = Ampere, 40 = Ada Lovelace, 50 = Blackwell). The last two digits place the card within its series: in the RTX 50 Series a higher number has more CUDA cores, from the RTX 5050 to the RTX 5090. Data center: a letter and a number (A100, H100, B200); NVIDIA publishes no meaning for the number.'
suffixes:
- symbol: Ti
  meaning: A card above the same-numbered model in its series; the RTX 5070 Ti has 8,960 CUDA cores against 6,144 on the RTX 5070
- symbol: SUPER
  meaning: A later version of an existing card; NVIDIA's RTX 40 SUPER Series (January 2024) has more cores than the cards it shares a number with
- symbol: SXM / NVL
  meaning: 'Data center form factor on the H100 page: H100 SXM is an SXM module; H100 NVL is a dual-slot PCIe card'
examples:
- name: GeForce RTX 4090
  parts:
  - token: RTX
    explains: GeForce RTX consumer line
  - token: '40'
    explains: RTX 40 Series, the Ada Lovelace architecture
  - token: '90'
    explains: The highest number in the RTX 40 Series
- name: GeForce RTX 4080 SUPER
  parts:
  - token: RTX
    explains: GeForce RTX consumer line
  - token: '40'
    explains: RTX 40 Series, the Ada Lovelace architecture
  - token: '80'
    explains: Position within the series, below the RTX 4090
  - token: SUPER
    explains: Later version of the RTX 4080 with more cores (announced January 2024)
- name: H100 SXM
  parts:
  - token: H
    explains: Hopper architecture
  - token: '100'
    explains: Model number
  - token: SXM
    explains: SXM module form factor (the H100 NVL is the PCIe card)
tags:
- nvidia
- naming
- geforce
- datacenter
updated: '2026-11-21'
sources:
- url: https://www.nvidia.com/en-us/geforce/graphics-cards/compare/
  title: NVIDIA — Compare GeForce Graphics Cards
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/10-years-in-the-making-nvidia-brings-real-time-ray-tracing-to-gamers-with-geforce-rtx
  title: NVIDIA — GeForce RTX 20 Series announcement (20 August 2018)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-introduces-the-beastly-geforce-gtx-1080-ti-fastest-gaming-gpu-ever
  title: NVIDIA — GeForce GTX 1080 Ti announcement (28 February 2017)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/geforce-rtx-40-super-series
  title: NVIDIA — GeForce RTX 40 SUPER Series announcement (8 January 2024)
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/h100/
  title: NVIDIA H100 Tensor Core GPU
  trust: 0.95
- url: https://www.nvidia.com/en-us/data-center/l40s/
  title: NVIDIA L40S GPU
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidias-new-ampere-data-center-gpu-in-full-production
  title: NVIDIA — A100 announcement (14 May 2020)
  trust: 0.95
- url: https://nvidianews.nvidia.com/news/nvidia-blackwell-platform-arrives-to-power-a-new-era-of-computing
  title: NVIDIA — Blackwell platform announcement (18 March 2024)
  trust: 0.95
---

## How To Read

The prefix gives the line:

- **RTX** and **GTX** are consumer GeForce cards.
- A **letter and a number** (A100, H100, B200, L40S) is a data center GPU; for A, H and B the letter is the
  architecture's initial, while the L-series is Ada Lovelace.

For GeForce RTX, read the number as **series + position**: the leading digits give the series (40 = Ada
Lovelace, 50 = Blackwell) and the last two digits place the card within it. **Ti** marks a card above the
same-numbered model, and **SUPER** a later version with more cores. On the H100, **SXM** and **NVL** name the
form factor.
