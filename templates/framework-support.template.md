---
id: framework-support/<slug>
type: framework-support
slug: <slug>                       # the framework, e.g. pytorch, onnx-runtime
schema_version: 2.0
title: "<Framework name>"
checked: <YYYY-MM-DD>              # the day every platform source was last read
platforms:                         # only what the framework's (or the platform maker's) own page states
  - platform: cuda                 # cuda | rocm | apple-silicon | intel-gpu | intel-gaudi | google-tpu
    supported: true                # false only when the page says the platform is not supported
    min_compute_capability: 7.5    # optional, cuda only: the lowest compute capability the page names
    gpus: [gpu/<slug>]             # optional: when the page lists products, only these GPUs
    note: "<qualification the page states>"   # optional
    source: "<page URL>"           # also listed in sources
tags: [<slug>, framework-support]
updated: <YYYY-MM-DD>
sources:
  - { url: "<page URL>", title: "<title>", trust: 0.95 }
---
