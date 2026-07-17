---
id: glossary-term/die-size
type: glossary-term
slug: die-size
schema_version: 1.0
title: "Die Size and Reticle Limit"
term: "Die Size and Reticle Limit"
category: packaging
examples: ["~814 mm2 GH100 (Hopper), near the reticle limit", "Blackwell: two dies joined to exceed one reticle", "Chiplets: many small dies vs one big die"]
related: [glossary-term/process-node]
tags: [packaging, die-size, chiplet]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Die_(integrated_circuit)", title: "Die (integrated circuit) — Wikipedia", trust: 0.8 }
---

## Definition
Die size is the physical area of a chip. The reticle limit (~800+ mm²) is the largest area a lithography
machine can pattern in one exposure — a hard ceiling on how big a single monolithic die can be. Yield
falls as die size grows, since one defect can ruin a larger, costlier chip.

## Why You Care
The reticle limit is why the industry turned to chiplets and multi-die packaging: AMD's MI300 and RDNA 3
and NVIDIA's Blackwell all stitch multiple dies together to exceed what one die can do, while improving
yield by using smaller dies. Understanding this explains a major recent architectural theme — "more
performance" increasingly means "more dies working as one," not "one bigger die."
