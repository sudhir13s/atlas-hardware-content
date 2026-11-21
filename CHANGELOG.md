# Changelog

All notable changes to `ai-hardware-content`. Grouped by schema version / release. Follows
[Keep a Changelog](https://keepachangelog.com/) conventions.

## [Unreleased]

### Accuracy pass (2026-11-21)

- **Changed** every architecture, timeline, glossary, name-decoder, upgrade-path and guide record so
  each statement rests on a maker page, standards-body page or original paper listed in `sources`;
  Wikipedia sources and statements without a primary source were removed.
- **Changed** `representative_gpus` in the architecture records to hold only slugs of records in
  `gpus/`; other products are named in the What Changed text where a maker page confirms them.
- **Removed** superlatives, unattributed "first" claims and folklore name-decoder meanings;
  maker claims that stay are attributed to the maker.
- **Changed** the guide rules of thumb to shown arithmetic from sourced inputs, labelled as estimates.

### Schema 1.3 (maker launch prices)

- **Added** the optional `gpu` fields `market.msrp_source` (the maker page that states the price) and
  `market.msrp_announced` (its date); `msrp_usd` now holds only a maker-published launch price, set
  from the maker's page on 7 consumer records and removed from the 26 whose maker published none.

### Schema 1.2 (the Buying Guide page reads the guide records)

- **Changed** the `guide` type to the blocks the page shows: required `page_section`
  (`quick-decision`, `background`, `power`, `further-reading`) and `order`; lists `decisions`
  (`scenario`, `recommendation`, optional `section`), `mistakes`, `points` (`name`, `text`) and one
  `table` (`columns`, `rows`). `title` is the heading shown; Overview and Takeaway are the lead-in
  and the closing rule.
- **Removed** the guide fields `vram_by_model_size`, `rules_of_thumb`, `memory_technologies`,
  `ecosystems`, `quantization_methods`, `interconnects`, `power_costs`, `decision_flowchart` and the
  `icon` of a decision: the page computes memory and power figures from the GPU records and shows
  none of the others.
- **Changed** the wording of the seven kept guide records to the page's wording, which carries no
  price or spec figure without a source (the 1.1 text had unsourced dollar amounts).
- **Added** the `further-reading` guide record (outside links, kept in `sources`).
- **Removed** the `vram` guide record: the page leaves VRAM to the `vram` glossary term.

### Schema 1.1 (migration of the GPU snapshot and the buying guide)

- **Added** the `gpu` type (`gpus/`, `gpu/<slug>`): `vendor` (NVIDIA, AMD, Intel, Apple, Google),
  `segment`, `series`, `generation`, `release_date`, `signal_strength`, `summary`, `aliases`,
  `specifications` (structured: `interconnect`, `process_node`, `form_factor[]`, numeric `pcie_gen`,
  `unit_kind` / `gpus_per_module`, `memory_kind`, `memory_bandwidth_gb_per_s`), `performance`,
  `ml_capabilities` (with structured `multi_gpu_scaling`), `framework_support`, the agent-owned
  `market` block, label lists and `image`; optional body section Overview.
- **Added** the `guide` type (`guides/`, `guide/<slug>`): `order` plus the section's tables and
  lists as rows of strings; optional body sections Overview and Takeaway.
- **Added** the shared optional `locked` field (field paths no job may change) to every type.
- **Added** 44 `gpu` records (one per GPU of the snapshot, built by code, no model call) and 8
  `guide` records (the buying advice, copied word for word from the guide page).

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
- **1.1** — `gpu` and `guide` types, shared `locked`.
- **1.2** — `guide` reshaped to the blocks of the Buying Guide page.
- **1.3** — `gpu` `market.msrp_source` and `market.msrp_announced`.
