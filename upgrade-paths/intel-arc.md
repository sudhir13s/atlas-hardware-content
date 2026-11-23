---
id: upgrade-path/intel-arc
type: upgrade-path
slug: intel-arc
schema_version: 3.0
title: Intel discrete GPUs (Xe → Arc)
vendor: Intel
family: Arc / Xe (consumer discrete)
steps:
- gpu_name: Iris Xe MAX Graphics (DG1)
  architecture_id: gpu-architecture/xe
  year: 2020
- gpu_id: gpu/intel-arc-a770
  architecture_id: gpu-architecture/xe-hpg
  year: 2022
tags:
- intel
- arc
- xe
- consumer
updated: '2026-11-21'
sources:
- url: https://download.intel.com/newsroom/archive/Geos/LatinAmerica/La-innovaci-n-se-ampl-a-con-los-gr-ficos-Intel-Iris-Xe-MAX-y-Deep-Link--English-Only-_10-31-2020_15-16.pdf
  title: Intel — Intel Iris Xe MAX graphics introduction (31 October 2020)
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/developer/articles/technical/introduction-to-the-xe-hpg-architecture.html
  title: Intel — Introduction to the Xe-HPG Architecture
  trust: 0.95
- url: https://www.intel.com/content/www/us/en/products/sku/229151/intel-arc-a770-graphics-16gb/specifications.html
  title: Intel — Intel Arc A770 Graphics (16GB)
  trust: 0.95
---

## Overview

Intel's discrete GPUs, from Xe to Arc:

- **Intel Iris Xe MAX graphics** (code-named DG1), introduced on 31 October 2020, which Intel describes
  as its first Xe-based discrete GPU.
- **Arc A770** (Xe-HPG), with Intel Xe Matrix Extensions (XMX) engines and ray tracing units.
