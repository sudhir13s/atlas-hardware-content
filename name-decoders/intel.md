---
id: name-decoder/intel
type: name-decoder
slug: intel
schema_version: 1.0
title: "Intel product-name decoder"
vendor: Intel
prefixes:
  - { symbol: "Arc", meaning: "Consumer discrete GPU brand" }
  - { symbol: "Gaudi", meaning: "Datacenter AI accelerator (from Habana Labs)" }
numbering: "Arc: a generation letter (A = Alchemist, B = Battlemage) followed by three digits whose leading digit is the tier class (A7xx = high, A5xx = mid, A3xx = entry). Gaudi: a single generation number (Gaudi 2, Gaudi 3)."
suffixes:
  - { symbol: "Limited Edition", meaning: "Intel's own first-party board design" }
examples:
  - name: "Arc A770"
    parts:
      - { token: "Arc", explains: "Consumer discrete GPU brand" }
      - { token: "A", explains: "Alchemist generation (Xe-HPG)" }
      - { token: "770", explains: "7-class = high tier; the 70 identifies the specific SKU" }
  - name: "Gaudi 3"
    parts:
      - { token: "Gaudi", explains: "Datacenter AI training/inference accelerator" }
      - { token: "3", explains: "Third generation (5nm, adds FP8)" }
tags: [intel, naming, arc, gaudi]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Intel_Arc", title: "Intel Arc — Wikipedia", trust: 0.8 }
---

## How To Read
The prefix names the product family: **Arc** for consumer discrete GPUs, **Gaudi** for datacenter AI
accelerators. For **Arc**, a **generation letter** comes first (A = Alchemist, B = Battlemage), then three
digits whose **leading digit is the performance class** (7 = high, 5 = mid, 3 = entry). For **Gaudi**, the
name is just the brand plus a **generation number** (Gaudi 2, Gaudi 3), each step advancing the process
node and precision support (Gaudi 3 adds FP8).
