---
id: name-decoder/<slug>
type: name-decoder
slug: <slug>
schema_version: 3.0              # the schema's current version; the schema refuses any other
title: "<Vendor> product-name decoder"
vendor: NVIDIA                     # NVIDIA | AMD | Intel
prefixes:
  - { symbol: "<prefix>", meaning: "<what it signals>" }
numbering: "<how the number encodes generation + tier>"
suffixes:
  - { symbol: "<suffix>", meaning: "<what it signals>" }
examples:
  - name: "<Full Product Name>"
    parts:
      - { token: "<token>", explains: "<what this part means>" }
tags: [<tag>]
updated: <YYYY-MM-DD>
sources:
  - { url: "<url>", title: "<title>", trust: 0.9 }
---

## How To Read
<Walk through how to parse a product name in this vendor's scheme.>
