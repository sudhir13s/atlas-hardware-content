# CONVENTIONS.md — authoring rules

The rules every file follows. Humans and agents follow the identical process. The authoritative
cross-repo spec is the
[content-repo standard](https://github.com/sudhir13s/TheAIAtlas/blob/main/docs/content-repo-standard.md);
this file is the `hardware`-domain instance.

## Slugs and file names

- Slugs are **lowercase, hyphen-separated, ASCII** — no spaces, no underscores. Example:
  `ada-lovelace`, `rdna-3`, `tensor-core`, `nvidia-datacenter`.
- The file name is `<slug>.md` and **must equal** the `slug` frontmatter field.
- A file lives in the folder mapped to its `type` in `schema/registry.json`.

## IDs

- `id` = `<type>/<slug>` (e.g. `gpu-architecture/hopper`). Globally unique, **immutable**.
- All cross-references use IDs, never titles:
  - `predecessor`, `successor` → `gpu-architecture/<slug>`
  - `architecture_id` (timeline events), `steps[].architecture_id` (upgrade paths) → `gpu-architecture/<slug>`
  - `related` (glossary) → `glossary-term/<slug>`
- `gpu_id` and `steps[].gpu_id` are **free-form product strings** (e.g. `"H100 SXM"`), not IDs.
- Every referenced ID must resolve to an existing file. Dangling references fail validation.

## Frontmatter

Base fields on **every** file: `id`, `type`, `slug`, `schema_version`, `title`, `tags`, `updated`,
`sources`. Optional base field: `related`. Each type adds its own fields — see
`schema/<type>.schema.json`. Put **structured/reference data in frontmatter** (arrays, spec fields,
step lists) so it stays machine-parseable.

- `tags`: lowercase, hyphen-separated.
- `updated`: ISO date (`YYYY-MM-DD`).
- `sources[]`: `{ url, title, trust }` — `trust` in `[0,1]`. Open-source-first; cite, do not copy.
- `schema_version`: the `major.minor` the file was authored against (currently `1.0`).

## Body sections

- Prose lives under `##` headings. The **required sections** and their order per type are declared
  in `schema/registry.json → types.<type>.sections`.
- The body carries the human-facing prose field that the consumer renders:
  - `gpu-architecture` → `What Changed` (the whole "what this generation changed" narrative)
  - `timeline-event` → `Description`
  - `glossary-term` → `Definition` and `Why You Care`
  - `upgrade-path` → `Overview`
  - `name-decoder` → `How To Read`
  - `gpu` → optional `Overview` (the `summary`, verbatim)
  - `guide` → optional `Overview` (lead-in) and `Takeaway` (closing rule or footnote)

## Per-type specifics

- **gpu** — one file per product, slug = the product's catalog id (`nvidia-h100-sxm`). Everything
  that is a number or a unit is a field, never text: `specifications` (`memory_gb`,
  `memory_bandwidth_gb_per_s`, `tdp_watts`, `form_factor[]`, `pcie_gen`, `interconnect`
  `{name, bandwidth_gb_per_s?, note?}`, `process_node` `{nodes_nm[], note?}`), `performance`
  (peak `*_tflops` / `int8_tops`), `ml_capabilities`, `framework_support`. A value the vendor does not
  publish is **absent**, never `0` or `"Unknown"`. `unit_kind: module` (with `gpus_per_module`) marks
  several GPUs sold as one unit: its memory, compute units and TDP cover the whole module.
  `memory_kind: unified` marks memory shared with the CPU. `market` is agent-owned (prices change)
  and carries `observed_at` and `source`. Body: Overview.
- **guide** — one file per advice section, `order` = position in the guide. Tables and lists are
  frontmatter lists of string rows (see the schema for each list's keys); lead-in and closing text
  are body sections. Wording is the guide's own and is changed only on purpose.

- **gpu-architecture** — one file per generation. Carries `vendor`, `year`, `process_node`,
  `segment`, `memory_tech`, `interconnect`, `key_innovation`, and the arrays `representative_gpus`,
  `innovations`, `precision_support`; plus `predecessor`/`successor` (IDs) forming the lineage DAG.
  Body: What Changed.
- **timeline-event** — a dated release or milestone. `event_type` is `release` | `milestone`
  (this is the consumer's `type` field; the frontmatter `type` is always `timeline-event`).
  Optional `architecture_id` (ID) and `gpu_id` (free string). Body: Description.
- **glossary-term** — `term`, `category`, `examples[]`, optional `related[]` (glossary IDs).
  Body: Definition → Why You Care.
- **upgrade-path** — `vendor`, `family`, and an ordered `steps[]` of
  `{ gpu_id, architecture_id, year }`. Body: Overview.
- **name-decoder** — `vendor`, `prefixes[]`, `numbering`, `suffixes[]`, and worked `examples[]` of
  `{ name, parts:[{token, explains}] }`. Body: How To Read.

## Sourcing

Open-source-first, zero plagiarism. Prefer vendor whitepapers, official architecture/spec pages,
and public references (e.g. Wikipedia for dates). Reference paywalled material only as a cited
pointer, never as copied text. Record everything in `sources[]`.
