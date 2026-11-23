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
  - `platforms[].gpus` (framework support) → `gpu/<slug>`
  - `framework` (framework support) → `framework/<slug>`, a record of the frameworks content repo
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
- `schema_version`: the `major.minor` the file was authored against; the repo's current version is in
  `meta.json` and `schema/registry.json`.

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
  (peak `*_tflops` / `int8_tops`, with `basis` `dense` or `sparse` when the maker states it),
  `ml_capabilities`. `compute_platform` names the acceleration platform frameworks target (`cuda`,
  `rocm`, `apple-silicon`, `intel-gpu`, `intel-gaudi`, `google-tpu`); `compute_capability` is
  NVIDIA's own figure (CUDA GPUs page or the architecture whitepaper). A value the vendor does not publish is **absent**, never
  `0` or `"Unknown"`; no field is kept only because it was once required. `release_date` is the
  maker's announced availability or launch date, and the announcement date only when the maker gives
  nothing more exact than a month or quarter. `unit_kind: module` (with `gpus_per_module`) marks
  several GPUs sold as one unit: its memory, compute units and TDP cover the whole module.
  `memory_kind: unified` marks memory shared with the CPU; such a record lists in
  `memory_options_gb` every memory size of the computers the maker sells with the chip (for Apple:
  Macs, not iPads; smallest first, read from their tech-spec pages, each cited in `sources`), and
  `memory_gb` is the largest of them. `market` is agent-owned (prices change)
  and carries `observed_at` and `source`. `msrp_usd` is only the maker's own published launch price
  (press release, newsroom post or product page), with that page in `msrp_source` and the
  announcement date in `msrp_announced`; no reseller, news or analyst figure, and absent when the
  maker published none (most datacenter parts; Apple chips, whose Macs carry the price). Body: Overview.
- **guide** — one file per block of the Buying Guide page: `page_section` says which page section
  shows it, `order` = position, `title` = the heading. Lists (`decisions`, `mistakes`, `points`) and
  the one `table` are frontmatter rows of strings (see the schema); lead-in and closing text are the
  body sections. A `further-reading` block keeps its links in `sources`. Wording is the guide's own
  and is changed only on purpose.
- **framework-support** — one file per framework (slug = the framework, e.g. `onnx-runtime`), no
  body. `platforms[]` lists each compute platform the framework's own page (or the platform maker's)
  states: `supported` (false only when the page says so), `source` (that page, also in `sources`),
  and when the page narrows it, `min_compute_capability` (cuda) or `gpus[]` (the listed products, as
  `gpu/<slug>` IDs) and a short `note`. `checked` is the day the pages were read. A GPU's support is
  derived from its `compute_platform`; a platform, product or compute capability the page does not
  name is unknown, never unsupported. `framework` names the `framework/<slug>` record of the same
  project when the frameworks content repo has one; that record's page shows these platforms, so
  the framework record stores no GPU support of its own.

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
