---
id: upgrade-path/<slug>
type: upgrade-path
slug: <slug>
schema_version: 3.0              # the schema's current version; the schema refuses any other
title: "<Path Title>"
vendor: NVIDIA                     # NVIDIA | AMD | Intel
family: "<e.g. Datacenter, GeForce (consumer)>"
steps:
  - { gpu_id: gpu/<slug>, architecture_id: gpu-architecture/<slug>, year: <YYYY> }           # the product has a record
  - { gpu_name: "<product or family>", architecture_id: gpu-architecture/<slug>, year: <YYYY> }   # it has none
tags: [<tag>]
updated: <YYYY-MM-DD>
sources:
  - { url: "<url>", title: "<title>", trust: 0.9 }
---

## Overview
<A sentence describing the generational upgrade path this represents.>
