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
  - `predecessors[]` (architectures), `architecture` (GPUs) → `gpu-architecture/<slug>`
  - `representative_gpus[]` (architectures), `gpu_id` (timeline events), `steps[].gpu_id`
    (upgrade paths) → `gpu/<slug>`
  - `architecture_id` (timeline events), `steps[].architecture_id` (upgrade paths) → `gpu-architecture/<slug>`
  - `related` (glossary) → `glossary-term/<slug>`
  - `platforms[].gpus` (framework support) → `gpu/<slug>`
  - `framework` (framework support) → `framework/<slug>`, a record of the frameworks content repo
- A product with no `gpu` record is written in `gpu_name` (`"Tesla V100"`), never in `gpu_id`;
  an event or a step has one or the other. A `gpu` record is not created to make a name an ID.
- **No stored reverse link.** An architecture lists what came before it; what came after is read
  from the records that name it.
- Every referenced ID must resolve to an existing file. Dangling references fail validation.

## Frontmatter

Base fields on **every** file: `id`, `type`, `slug`, `schema_version`, `title`, `tags`, `updated`,
`sources`. Optional base field: `related`. Each type adds its own fields — see
`schema/<type>.schema.json`. Put **structured/reference data in frontmatter** (arrays, spec fields,
step lists) so it stays machine-parseable.

- `tags`: lowercase, hyphen-separated.
- `updated`: ISO date (`YYYY-MM-DD`).
- `sources[]`: `{ url, title, trust }` — `trust` in `[0,1]`. Open-source-first; cite, do not copy.
- `schema_version`: the version of the type's schema. Every schema fixes the value (`3.0`) and a
  record with any other is refused; a breaking change raises it and converts every record.
- **No unknown fields** on any type, at the top level or inside a block of fixed shape.

## Body sections

- Prose lives under `##` headings. The **required sections** and their order per type are declared
  in `schema/registry.json → types.<type>.sections`.
- The body carries the human-facing prose field that the consumer renders:
  - `gpu-architecture` → `What Changed` (the whole "what this generation changed" narrative)
  - `timeline-event` → `Description`
  - `glossary-term` → `Definition` and `Why You Care`
  - `upgrade-path` → `Overview`
  - `name-decoder` → `How To Read`
  - `guide` → optional `Overview` (lead-in) and `Takeaway` (closing rule or footnote)

## Per-type specifics

- **gpu** — one file per product, slug = the product's catalog id (`nvidia-h100-sxm`). Everything
  that is a number or a unit is a field, never text: `specifications` (`memory_gb`,
  `memory_bandwidth_gb_per_s`, `tdp_watts`, `form_factor[]`, `pcie_gen`, `interconnect`
  `{name, bandwidth_gb_per_s?, note?}`, `process_node` `{nodes_nm[], note?}`), `performance`
  (peak `*_tflops` / `int8_tops`, dense and for one GPU or chip; a figure the maker gives only
  with sparsity is halved only when the maker states dense is half, and a figure given only per
  module is left out),
  `ml_capabilities`. `compute_platform` names the acceleration platform frameworks target (`cuda`,
  `rocm`, `apple-silicon`, `intel-gpu`, `intel-gaudi`, `google-tpu`). `segment: laptop` marks a GPU
  built into laptops, a separate record from the desktop card of the same name (slug ends in
  `-laptop`, title is the maker's "… Laptop GPU" name); the maker's power range for it, which the
  laptop maker sets, stays in `key_features`, never `tdp_watts`. `compute_capability` is
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
  maker published none (most datacenter parts; Apple chips, whose Macs carry the price).
  `generation` is the architecture as the maker names it and the text shown; `architecture` is the
  ID of the `gpu-architecture` record of that name, when there is exactly one. `series` is the
  product family and is absent when the maker names none besides the generation. No body section:
  the prose is `summary`, stored once.
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
  `innovations`, `precision_support`; plus `predecessors[]` (IDs, the direct line first) forming the
  lineage DAG.
  Body: What Changed.
- **timeline-event** — a dated release or milestone. `event_type` is `release` | `milestone`
  (this is the consumer's `type` field; the frontmatter `type` is always `timeline-event`).
  Optional `architecture_id` (ID) and the product: `gpu_id` (ID) or `gpu_name`. Body: Description.
- **glossary-term** — `term`, `category`, `examples[]`, optional `related[]` (glossary IDs).
  Body: Definition → Why You Care.
- **upgrade-path** — `vendor`, `family`, and an ordered `steps[]` of
  `{ gpu_id | gpu_name, architecture_id, year }`. Body: Overview.
- **name-decoder** — `vendor`, `prefixes[]`, `numbering`, `suffixes[]`, and worked `examples[]` of
  `{ name, parts:[{token, explains}] }`. Body: How To Read.

## Sourcing

Open-source-first, zero plagiarism. Prefer vendor whitepapers, official architecture/spec pages,
and public references (e.g. Wikipedia for dates). Reference paywalled material only as a cited
pointer, never as copied text. Record everything in `sources[]`.
