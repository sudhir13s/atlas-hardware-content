---
id: gpu-architecture/cdna-3
type: gpu-architecture
slug: cdna-3
schema_version: 1.0
title: "AMD CDNA 3"
name: "CDNA 3"
vendor: AMD
year: 2023
predecessor: gpu-architecture/cdna-2
process_node: "TSMC 5nm (XCD) + TSMC 6nm (IOD)"
segment: "datacenter"
representative_gpus: ["amd-mi300x", "amd-mi325x"]
key_innovation: "A 3D-stacked chiplet design (compute dies on I/O dies) built as discrete GPUs (MI300X, MI325X) or as an APU with Zen 4 CPU cores and unified HBM3 (MI300A)."
innovations: ["Accelerator complex dies (XCDs) stacked on I/O dies (IODs)", "AMD Infinity Cache (256 MB) on the I/O dies", "MI300A APU: 24 Zen 4 cores and CDNA 3 GPU sharing unified HBM3", "FP8 (E4M3, E5M2) and TF32 matrix support, plus sparsity", "4th Gen AMD Infinity Architecture"]
precision_support: ["FP64", "FP32", "TF32", "FP16", "BF16", "FP8", "INT8"]
memory_tech: "HBM3 (MI300X, MI300A) / HBM3E (MI325X)"
interconnect: "Infinity Fabric, PCIe 5.0"
tags: [amd, cdna-3, mi300x, mi300a, hbm3, fp8, apu]
updated: '2026-11-21'
sources:
  - { url: "https://www.amd.com/content/dam/amd/en/documents/instinct-tech-docs/white-papers/amd-cdna-3-white-paper.pdf", title: "AMD CDNA 3 Architecture white paper", trust: 0.95 }
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html", title: "AMD Instinct MI300X specifications", trust: 0.95 }
  - { url: "https://www.amd.com/en/products/accelerators/instinct/mi300/mi325x.html", title: "AMD Instinct MI325X specifications", trust: 0.95 }
  - { url: "https://www.amd.com/en/technologies/cdna.html", title: "AMD CDNA Architecture (generation table)", trust: 0.95 }
---

## What Changed
CDNA 3 powers the **Instinct MI300 Series**. The MI300X launched on 6 December 2023 and the MI325X on
10 October 2024.

- **3D stacking:** up to eight **accelerator complex dies (XCDs)** on TSMC 5nm sit on four **I/O dies**
  on TSMC 6nm, which hold the 256 MB Infinity Cache and the HBM interface.
- **Memory:** **192 GB HBM3** at 5.3 TB/s on MI300X; **256 GB HBM3E** at 6 TB/s on MI325X.
- **APU:** the **MI300A** swaps two XCDs for three Zen 4 CPU dies (24 cores) sharing one unified HBM3
  pool, which removes host-to-device copies. AMD calls it the first data center APU.
- **Precision:** matrix support adds **FP8** (E4M3 and E5M2) and **TF32**, plus sparsity.
- **Links:** seven Infinity Fabric links per MI300X connect eight GPUs; the host link is PCIe 5.0.
