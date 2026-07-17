---
id: timeline-event/<slug>
type: timeline-event
slug: <slug>
schema_version: 1.0
title: "<Event Title>"
date: <YYYY-MM-DD>                 # ISO date (year/month prefix allowed)
vendor: NVIDIA                     # NVIDIA | AMD | Intel
event_type: release               # release | milestone
architecture_id: gpu-architecture/<slug>   # optional; FK
gpu_id: "<free-form product id>"           # optional
tags: [<tag>]
updated: <YYYY-MM-DD>
sources:
  - { url: "<url>", title: "<title>", trust: 0.9 }
---

## Description
<One or two sentences on what happened and why it matters.>
