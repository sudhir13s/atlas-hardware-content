---
id: guide/power-cooling-tco
type: guide
slug: power-cooling-tco
schema_version: 1.1
title: Power, Cooling & Total Cost of Ownership
order: 6
power_costs:
- gpu: RTX 4090
  tdp: 450W
  electricity_per_year: ~$475
  cooling: Air (large case)
  psu_needed: 850W+
- gpu: RTX 5090
  tdp: 575W
  electricity_per_year: ~$605
  cooling: Air (large case)
  psu_needed: 1000W+
- gpu: A100 80GB
  tdp: 300W
  electricity_per_year: ~$315
  cooling: Server room
  psu_needed: Server PSU
- gpu: H100 SXM
  tdp: 700W
  electricity_per_year: ~$735
  cooling: Liquid cooling
  psu_needed: DGX/HGX system
- gpu: M4 Ultra
  tdp: ~125W
  electricity_per_year: ~$130
  cooling: Silent (passive)
  psu_needed: Integrated
tags:
- gpu-buying-guide
- power-cooling-tco
updated: '2026-11-19'
sources: []
---

## Overview

The sticker price is not the total cost. Factor in power consumption, cooling requirements, and electricity costs.

## Takeaway

*Assumes 24/7 usage at $0.12/kWh US average. Real costs vary by location and utilization rate.
