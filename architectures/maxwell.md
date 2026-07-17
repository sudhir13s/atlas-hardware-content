---
id: gpu-architecture/maxwell
type: gpu-architecture
slug: maxwell
schema_version: 1.0
title: "NVIDIA Maxwell"
name: "Maxwell"
vendor: NVIDIA
codename: "GM1xx / GM2xx"
year: 2014
predecessor: gpu-architecture/kepler
successor: gpu-architecture/pascal
process_node: "TSMC 28nm"
segment: "consumer + datacenter"
representative_gpus: ["GeForce GTX 750 Ti (2014)", "GeForce GTX 980 (2014)", "GeForce GTX 980 Ti (2015)", "Tesla M40 (2015)"]
key_innovation: "A redesigned SMM multiprocessor roughly doubled performance-per-watt on the same 28nm node as Kepler."
innovations: ["SMM power-efficient multiprocessor", "Much larger L2 cache to cut memory traffic", "Improved delta color compression", "Big performance-per-watt gain without a node shrink"]
precision_support: ["FP64", "FP32"]
memory_tech: "GDDR5"
interconnect: "PCIe 3.0"
tags: [nvidia, maxwell, cuda, efficiency]
updated: 2026-07-17
sources:
  - { url: "https://en.wikipedia.org/wiki/Maxwell_(microarchitecture)", title: "Maxwell (microarchitecture) — Wikipedia", trust: 0.8 }
  - { url: "https://developer.nvidia.com/maxwell-compute-architecture", title: "NVIDIA Maxwell Compute Architecture", trust: 0.95 }
---

## What Changed
Maxwell was an **efficiency generation**: stuck on the same TSMC 28nm process as Kepler, NVIDIA
extracted its gains from architecture rather than a node shrink. The SMM multiprocessor was
partitioned into smaller, more autonomous blocks with dedicated scheduling and a much larger L2
cache, cutting off-chip memory traffic and roughly doubling performance-per-watt. For AI this was an
incremental step — the Tesla M40 became a common inference and training card — but like Kepler it had
**no dedicated matrix hardware**. Maxwell's real significance was proving NVIDIA could deliver large
generational gains from design alone, setting up the FinFET jump that came with Pascal.
