---
id: glossary-term/tdp
type: glossary-term
slug: tdp
schema_version: 1.0
title: "TDP (Thermal Design Power)"
term: "TDP (Thermal Design Power)"
category: power
examples: ["450 W on RTX 4090", "700 W on H100 SXM", "~1000 W+ on a Blackwell B200 module"]
related: []
tags: [power, tdp, cooling]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Thermal_design_power", title: "Thermal design power — Wikipedia", trust: 0.8 }
---

## Definition
TDP is the amount of heat (in watts) a GPU is designed to dissipate under sustained load, used as a proxy
for its power draw and the cooling it requires. It is a design target, not a hard peak — transient spikes
can exceed it.

## Why You Care
TDP drives three practical things: the power supply and connectors you need, the cooling (air vs liquid)
and case airflow, and the electricity and data-center cooling bill at scale. Modern datacenter
accelerators pushing 700–1000+ W per module are why liquid cooling has become standard in AI racks, and
why "performance-per-watt," not just raw performance, is a first-order metric for large deployments.
