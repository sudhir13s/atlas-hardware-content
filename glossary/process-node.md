---
id: glossary-term/process-node
type: glossary-term
slug: process-node
schema_version: 1.0
title: "Process Node"
term: "Process Node"
category: packaging
examples: ["TSMC 4N (H100, Ada)", "Samsung 8N (Ampere GeForce)", "TSMC 5nm + 6nm chiplets (RDNA 3, MI300)"]
related: [glossary-term/die-size]
tags: [packaging, process-node, fabrication]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Semiconductor_device_fabrication", title: "Semiconductor device fabrication — Wikipedia", trust: 0.8 }
---

## Definition
A process node names the manufacturing technology a chip is fabricated on (e.g. "TSMC 4N", "Samsung 8nm").
Modern node names are marketing labels, not literal feature sizes, but a "smaller" node generally means
more transistors per area and better energy efficiency.

## Why You Care
The node largely determines how many transistors fit and how much power they burn, so a node shrink is
one of the biggest levers for generational performance-per-watt (e.g. Ampere GeForce on Samsung 8nm →
Ada on TSMC 4N). It also shapes cost and supply: leading-edge nodes are scarce and expensive, which is
why some vendors mix nodes (compute on the newest, memory/cache dies on an older one) via chiplets.
