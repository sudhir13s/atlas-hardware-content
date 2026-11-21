---
id: name-decoder/intel
type: name-decoder
slug: intel
schema_version: 1.0
title: "Intel product-name decoder"
vendor: Intel
prefixes:
  - { symbol: "Arc", meaning: "Intel Arc discrete GPUs" }
  - { symbol: "Gaudi", meaning: "Intel Gaudi AI accelerators for the data center" }
numbering: "Arc: a series letter and three digits. The A-series is the product family Intel formerly code-named Alchemist (Xe-HPG microarchitecture); the B-series, introduced on 3 December 2024, uses Intel's second-generation Xe core. Intel sells the A-series desktop GPUs as Intel Arc 3, 5 and 7 tiers, which it compares to Core i3, i5 and i7, and the leading digit matches the tier (A380, A580, A770). Gaudi: the brand and a generation number (Gaudi 2 is the second generation, Gaudi 3 the third)."
suffixes:
  - { symbol: "Limited Edition", meaning: "Intel's own Intel-branded card, as opposed to add-in-card partner boards" }
examples:
  - name: "Arc A770"
    parts:
      - { token: "Arc", explains: "Intel Arc discrete GPU brand" }
      - { token: "A", explains: "A-series, formerly code-named Alchemist (Xe-HPG)" }
      - { token: "770", explains: "Leading 7 = the Intel Arc 7 tier" }
  - name: "Gaudi 3"
    parts:
      - { token: "Gaudi", explains: "Intel Gaudi AI accelerator brand" }
      - { token: "3", explains: "Third generation; made on a TSMC 5 nm process, against 7 nm for Gaudi 2" }
tags: [intel, naming, arc, gaudi]
updated: '2026-11-21'
sources:
  - { url: "https://game.intel.com/us/stories/intel-arc-graphics-qa-hardware-specs", title: "Intel Gaming Access — Intel Arc Graphics Q&A: Hardware Specs Explained", trust: 0.95 }
  - { url: "https://www.intel.com/content/www/us/en/products/details/discrete-gpus/arc/desktop/a-series.html", title: "Intel Arc A-Series Graphics for Desktops", trust: 0.95 }
  - { url: "https://www.intel.com/content/www/us/en/developer/articles/technical/introduction-to-the-xe-hpg-architecture.html", title: "Intel — Introduction to the Xe-HPG Architecture", trust: 0.95 }
  - { url: "https://www.intel.com/content/www/us/en/newsroom/news/intel-launches-arc-b-series-graphics-cards.html", title: "Intel — Intel Launches Arc B-Series Graphics Cards", trust: 0.95 }
  - { url: "https://cdrdv2-public.intel.com/817486/gaudi-3-ai-accelerator-white-paper.pdf", title: "Intel Gaudi 3 AI Accelerator white paper", trust: 0.95 }
  - { url: "https://habana.ai/wp-content/uploads/2023/10/HL-225B_Datasheet_10_23.pdf", title: "Intel Gaudi 2 AI Accelerator HL-225B data sheet", trust: 0.95 }
---

## How To Read
The prefix names the family: **Arc** for discrete GPUs, **Gaudi** for data center AI accelerators.

- **Arc:** a **series letter** comes first (A = the family formerly code-named Alchemist), then three digits
  whose **leading digit is the Intel Arc tier** (3, 5 or 7). **Limited Edition** marks Intel's own card.
- **Gaudi:** the brand and a **generation number** (Gaudi 2, Gaudi 3).
