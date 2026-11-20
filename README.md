# atlas-hardware-content

Portable, reusable reference knowledge about **AI hardware** — GPU and accelerator generations,
their release timeline, the vocabulary you need to read a spec sheet, vendor upgrade paths, and
product-name decoders. Authored as Markdown with structured YAML frontmatter, validated by JSON
Schema, and readable by both humans and AI agents. This repo is **content only**: no code, no
build step, no framework lock-in. Any project can vendor it (as a git submodule or a plain
checkout) and render it however it likes.

It is the `hardware` domain of a multi-repo reference library
(`atlas-models-content`, `atlas-evaluation-content`, `atlas-frameworks-content`,
`atlas-hardware-content`, `atlas-news-content`, `atlas-practices-content`, `atlas-research-content`), all following the same
[content-repo standard](CONTENT-STANDARD.md).

## What's inside

| Type | Folder | What it captures |
|------|--------|------------------|
| `gpu` | `gpus/` | One GPU or accelerator (44 of them, NVIDIA, AMD, Intel, Apple, Google): structured specifications (memory, compute units, interconnect, process node, form factor), peak performance, ML capabilities, framework support, and an agent-owned `market` block (price, cloud rental) |
| `guide` | `guides/` | One section of the GPU buying advice (VRAM, memory bandwidth, quantization, power and cost, common mistakes, …) with its tables and lists as rows |
| `gpu-architecture` | `architectures/` | A GPU/accelerator generation: process node, memory, interconnect, key innovation, precision support, and predecessor/successor lineage |
| `timeline-event` | `timeline/` | A dated release or milestone (H100, MI300X, Blackwell, first Tensor Cores, …), linked to its architecture |
| `glossary-term` | `glossary/` | A plain-English definition of a hardware term (Tensor Core, HBM, NVLink, FP8, TDP, MIG, …) with "why you care" |
| `upgrade-path` | `upgrade-paths/` | An ordered vendor progression (V100 → A100 → H100 → B200), each step tied to a GPU + architecture + year |
| `name-decoder` | `name-decoders/` | How to parse a product name (RTX 4090, RX 7900 XTX, Arc A770) into prefix / number / suffix meaning |

## Quick start

```bash
# Vendor it
git clone https://github.com/sudhir13s/atlas-hardware-content.git
# or as a submodule of your project
git submodule add https://github.com/sudhir13s/atlas-hardware-content.git content/atlas-hardware-content
```

Every content file is a Markdown file with YAML frontmatter (the structured fields) and a Markdown
body (prose). Enumerate the library by globbing `**/*.md` and reading each file's frontmatter, or
start from [`meta.json`](meta.json) and [`schema/registry.json`](schema/registry.json).

## Structure

```
meta.json                 # repo descriptor (machine entrypoint 1)
schema/registry.json      # type → folder/schema/sections map (machine entrypoint 2)
schema/*.schema.json      # JSON Schema per content type
templates/*.template.md   # copy these to author new content
gpus/ guides/ architectures/ timeline/ glossary/ upgrade-paths/ name-decoders/
assets/                   # SVG diagrams
```

## Contributing

See [CONVENTIONS.md](CONVENTIONS.md) for the authoring rules, and [AGENTS.md](AGENTS.md) for the
machine-navigation guide. In short: copy a template, fill the frontmatter and required sections,
use IDs (not titles) for links, and open a PR. Content must be open-source-sourced and cited —
vendor whitepapers, official spec pages, and public references — never copied from paywalled
material.

## License

Content is licensed **CC-BY-4.0** (see [LICENSE](LICENSE)) — reuse freely with attribution.
