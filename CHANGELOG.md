# Changelog

All notable changes to `ai-hardware-content`. Grouped by schema version / release. Follows
[Keep a Changelog](https://keepachangelog.com/) conventions.

## [Unreleased]

### Added
- Repository scaffold to the content-repo standard: `meta.json`, `schema/registry.json`, the six
  JSON Schemas (`_shared`, `gpu-architecture`, `timeline-event`, `glossary-term`, `upgrade-path`,
  `name-decoder`), templates, and docs (`README`, `AGENTS`, `CONVENTIONS`).
- Initial GPU/accelerator content library (schema version 1.0), all cited and cross-link-validated:
  - **19 GPU architectures** — NVIDIA (Kepler → Blackwell), AMD (GCN, RDNA 1–3, CDNA 1–3), and
    Intel (Xe, Xe-HPG/Arc, Gaudi), with resolvable `predecessor`/`successor` lineage.
  - **21 timeline events** — key releases (V100, A100, H100, H200, MI100/250X/300X, RTX 30/40/50,
    RX 6000/7000, Arc A770, Blackwell) and milestones (first Tensor Cores, first RT Cores, FP8 +
    Transformer Engine), each linked to its architecture.
  - **20 glossary terms** — Tensor Core, CUDA Core, HBM, GDDR6, VRAM, memory bandwidth, NVLink,
    NVSwitch, PCIe, TDP, FP8, BF16, sparsity, TFLOPS, process node, MIG, Transformer Engine,
    RT Core, ROCm, die size.
  - **5 upgrade paths** — NVIDIA datacenter + GeForce, AMD Instinct + Radeon, Intel Arc.
  - **3 name decoders** — NVIDIA, AMD, Intel product-name schemes.

## Schema versions

- **1.0** — initial schema for all five hardware content types.
