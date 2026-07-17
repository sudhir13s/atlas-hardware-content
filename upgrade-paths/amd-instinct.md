---
id: upgrade-path/amd-instinct
type: upgrade-path
slug: amd-instinct
schema_version: 1.0
title: "AMD Instinct datacenter accelerators"
vendor: AMD
family: "Instinct (datacenter)"
steps:
  - { gpu_id: "Instinct MI100", architecture_id: gpu-architecture/cdna, year: 2020 }
  - { gpu_id: "Instinct MI250X", architecture_id: gpu-architecture/cdna-2, year: 2021 }
  - { gpu_id: "Instinct MI300X", architecture_id: gpu-architecture/cdna-3, year: 2023 }
tags: [amd, instinct, datacenter]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/AMD_Instinct", title: "AMD Instinct — Wikipedia", trust: 0.8 }
---

## Overview
AMD's datacenter accelerator line on the compute-only CDNA architecture: from the first Matrix Cores
(MI100), to a dual-die exascale HPC part (MI250X), to the 192 GB HBM3 AI accelerator (MI300X) that made
AMD a credible alternative to NVIDIA for large-model inference.
